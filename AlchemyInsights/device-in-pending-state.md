---
title: 保留状態のデバイス
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/11/2020
ms.locfileid: "49680549"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="06074-102">保留状態のデバイス</span><span class="sxs-lookup"><span data-stu-id="06074-102">Device in pending state</span></span>

<span data-ttu-id="06074-103">**前提条件:**</span><span class="sxs-lookup"><span data-stu-id="06074-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="06074-104">初めてデバイス登録を設定する場合は、[Azure Active Directory (Azure AD) でのデバイス管理の概要](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support)を確認してください。このガイドでは、デバイスを Azure AD の制御下に配置する方法について説明しています。</span><span class="sxs-lookup"><span data-stu-id="06074-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="06074-105">デバイスを Azure AD に直接登録し、それらを Intune に登録する場合は、[構成済み Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) があり、最初に[ライセンス](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support)が設定されていることを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="06074-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="06074-106">Azure AD およびオンプレミス AD で操作を実行する権限があることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="06074-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="06074-107">デバイス登録の設定を管理できるのは、Azure AD のグローバル管理者のみです。</span><span class="sxs-lookup"><span data-stu-id="06074-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="06074-108">さらに、オンプレミスの Active Directory で自動登録を設定する場合は、Active Directory と AD FS (該当する場合) の管理者である必要があります。</span><span class="sxs-lookup"><span data-stu-id="06074-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="06074-109">Hybrid Azure AD Join の登録プロセスを実行するには、デバイスが企業ネットワーク上にある必要があります。</span><span class="sxs-lookup"><span data-stu-id="06074-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="06074-110">VPN を経由して実行することもできますが、それにはいくつかの注意事項があります。</span><span class="sxs-lookup"><span data-stu-id="06074-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="06074-111">リモートワークのお客様のご要望にお応えして、Hybrid Azure AD Join の登録プロセスをトラブルシューティングするためのサポートを提供します。</span><span class="sxs-lookup"><span data-stu-id="06074-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="06074-112">**クラウド認証環境 (Azure AD パスワード ハッシュ同期またはパススルー認証の使用)**</span><span class="sxs-lookup"><span data-stu-id="06074-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="06074-113">この登録フローは "同期参加" とも呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="06074-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="06074-114">次に、登録プロセス中に発生する現象の詳細を示します。</span><span class="sxs-lookup"><span data-stu-id="06074-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="06074-115">Windows 10 は、ユーザーがデバイスにログオンすると、サービス接続ポイント (SCP) レコードを検出します。</span><span class="sxs-lookup"><span data-stu-id="06074-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="06074-116">まず、デバイスはクライアント側の SCP からの情報をレジストリ [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD] に取得しようとします。</span><span class="sxs-lookup"><span data-stu-id="06074-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="06074-117">詳細については、「[ドキュメント](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="06074-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="06074-118">失敗した場合、デバイスは社内 Active Directory と通信し、SCP からテナント情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="06074-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="06074-119">SCP を検証するには、この[ドキュメント](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="06074-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="06074-120">Active Directory で SCP を有効にし、クライアント側の SCP は最初の認証のときだけに使用することをおすすめします。</span><span class="sxs-lookup"><span data-stu-id="06074-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="06074-121">Windows 10 は Azure AD から認証を受けるために、システム コンテキストのもとで Azure AD との通信を試みます。</span><span class="sxs-lookup"><span data-stu-id="06074-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="06074-122">デバイスがシステム アカウントで Microsoft リソースにアクセスできるかどうかは、[テスト デバイス登録接続スクリプト](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)を使用して検証できます。</span><span class="sxs-lookup"><span data-stu-id="06074-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="06074-123">Windows 10 は自己署名証明書を生成し、社内 Active Directory のコンピューター オブジェクトに格納します。</span><span class="sxs-lookup"><span data-stu-id="06074-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="06074-124">これにはドメイン コントローラーまでの照準線が必要です。</span><span class="sxs-lookup"><span data-stu-id="06074-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="06074-125">証明書があるデバイス オブジェクトは、Azure AD Connect を経由して Azure AD に同期されます。</span><span class="sxs-lookup"><span data-stu-id="06074-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="06074-126">同期サイクルは既定で 30 分間隔ですが、Azure AD Connect の構成によって異なります。</span><span class="sxs-lookup"><span data-stu-id="06074-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="06074-127">詳細については、この[ドキュメント](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="06074-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="06074-128">この時点で、当該のデバイスが Azure ポータルのデバイス ブレードに「**保留中**」の状態で表示されるようになります。</span><span class="sxs-lookup"><span data-stu-id="06074-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="06074-129">ユーザーが次回 Windows 10 にログインするときに、登録が完了します。</span><span class="sxs-lookup"><span data-stu-id="06074-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="06074-130">デバイスが VPN 上にあり、ログオフとログインがドメイン接続を終了させる場合、手動で登録を開始することができます。</span><span class="sxs-lookup"><span data-stu-id="06074-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="06074-131">それには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="06074-131">To do that:</span></span>
    >
    > <span data-ttu-id="06074-132">`dsregcmd /join` をローカルで管理者プロンプトに、または PSExec からリモートで PC に発行します。</span><span class="sxs-lookup"><span data-stu-id="06074-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="06074-133">例: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="06074-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="06074-134">Azure Active Directory デバイス登録に関する一般的な問題については、「[デバイスに関する FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="06074-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
