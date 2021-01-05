---
title: PRT 問題のトラブルシューティング
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573963"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="013b7-102">PRT 問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="013b7-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="013b7-103">デバイスの認証を完了するには、完全に登録され、良好な状態で、プライマリ更新トークン (PRT) を取得できる必要があります。</span><span class="sxs-lookup"><span data-stu-id="013b7-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="013b7-104">Hybrid Azure AD Join の登録プロセスを実行するには、デバイスが企業ネットワーク上にある必要があります。</span><span class="sxs-lookup"><span data-stu-id="013b7-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="013b7-105">VPN を経由して実行することもできますが、それにはいくつかの注意事項があります。</span><span class="sxs-lookup"><span data-stu-id="013b7-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="013b7-106">リモートワークのお客様のご要望にお応えして、Hybrid Azure AD Join の登録プロセスをトラブルシューティングするためのサポートを提供します。</span><span class="sxs-lookup"><span data-stu-id="013b7-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="013b7-107">ここでは、登録プロセスの裏側で何が起きているかの概要を示します。</span><span class="sxs-lookup"><span data-stu-id="013b7-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="013b7-108">**クラウド認証環境 (Azure AD パスワード ハッシュ同期またはパススルー認証の使用)**</span><span class="sxs-lookup"><span data-stu-id="013b7-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="013b7-109">この登録フローは "同期参加" とも呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="013b7-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="013b7-110">Windows 10 は、ユーザーがデバイスにログオンするときに SCP レコードを検出します。</span><span class="sxs-lookup"><span data-stu-id="013b7-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="013b7-111">まず、デバイスはクライアント側の SCP からの情報をレジストリ [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD] に取得しようとします。</span><span class="sxs-lookup"><span data-stu-id="013b7-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="013b7-112">詳細については、この[ドキュメント](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="013b7-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="013b7-113">失敗した場合、デバイスは社内 Active Directory (AD) と通信し、サービス接続ポイント (SCP) からテナント情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="013b7-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="013b7-114">SCP を検証するには、この[ドキュメント](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="013b7-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="013b7-115">AD で SCP を有効にし、クライアント側の SCP は最初の認証のときだけに使用することをおすすめします。</span><span class="sxs-lookup"><span data-stu-id="013b7-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="013b7-116">Windows 10 は Azure AD から認証を受けるために、システム コンテキストのもとで Azure AD との通信を試みます。</span><span class="sxs-lookup"><span data-stu-id="013b7-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="013b7-117">デバイスがシステム アカウントで Microsoft リソースにアクセスできるかどうかは、テスト デバイス登録接続スクリプトを使用して検証できます。</span><span class="sxs-lookup"><span data-stu-id="013b7-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="013b7-118">Windows 10 は自己署名証明書を生成し、社内 AD のコンピューター オブジェクトに格納します。</span><span class="sxs-lookup"><span data-stu-id="013b7-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="013b7-119">これにはドメイン コントローラーまでの照準線が必要です。</span><span class="sxs-lookup"><span data-stu-id="013b7-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="013b7-120">証明書があるデバイス オブジェクトは、Azure AD Connect を経由して Azure AD に同期されます。</span><span class="sxs-lookup"><span data-stu-id="013b7-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="013b7-121">同期サイクルは既定で 30 分間隔ですが、Azure AD Connect の構成によって異なります。</span><span class="sxs-lookup"><span data-stu-id="013b7-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="013b7-122">詳細については、この[ドキュメント](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="013b7-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="013b7-123">この時点で、当該のデバイスが Azure ポータルのデバイス ブレードに "保留中" の状態で表示されるようになります。</span><span class="sxs-lookup"><span data-stu-id="013b7-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="013b7-124">ユーザーが次回 Windows 10 にログインするときに、登録が完了します。</span><span class="sxs-lookup"><span data-stu-id="013b7-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="013b7-125">デバイスが VPN 上にあり、ログオフとログインのプロセスがドメイン接続を終了させる場合、手動で登録を開始することができます。</span><span class="sxs-lookup"><span data-stu-id="013b7-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="013b7-126">dsregcmd /join をローカルで管理者プロンプトに、または PSExec からリモートで PC に発行します。</span><span class="sxs-lookup"><span data-stu-id="013b7-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="013b7-127">例: PsExec -s \\win10client01 cmd、dsregcmd /join</span><span class="sxs-lookup"><span data-stu-id="013b7-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="013b7-128">ハイブリッド参加の問題の詳細については、「[デバイスの問題のトラブルシューティング](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="013b7-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
