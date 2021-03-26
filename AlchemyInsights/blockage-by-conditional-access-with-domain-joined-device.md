---
title: ドメイン参加済みのデバイスで条件付きアクセスによりブロックされる
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/20/2021
ms.locfileid: "51038353"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="b53fc-102">ドメイン参加済みのデバイスで条件付きアクセスによりブロックされる</span><span class="sxs-lookup"><span data-stu-id="b53fc-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="b53fc-103">**強くお勧めするツール**</span><span class="sxs-lookup"><span data-stu-id="b53fc-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="b53fc-104">[デバイス登録トラブルシューティング ツール](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - 最も一般的なデバイス登録の問題に関するトラブルシューティングに役立つツールです。</span><span class="sxs-lookup"><span data-stu-id="b53fc-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="b53fc-105">[テスト デバイス登録接続スクリプト](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - デバイスがシステム アカウントでデバイス登録エンドポイントにアクセスできるようにするのに役立つスクリプトです。</span><span class="sxs-lookup"><span data-stu-id="b53fc-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="b53fc-106">[Azure AD デバイス クリーンアップ スクリプト](https://github.com/mzmaili/AzureADDeviceCleanup) - お使いの環境で古いデバイスを探して管理できるようにするためのスクリプトです。</span><span class="sxs-lookup"><span data-stu-id="b53fc-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="b53fc-107">ドメインに参加しているデバイス (Hybrid Azure AD) が条件付きアクセスで失敗するおそれがある一般的な理由を以下に示します。</span><span class="sxs-lookup"><span data-stu-id="b53fc-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="b53fc-108">**デバイス上に Azure AD PRT がない。** - デバイスが Azure AD プライマリ更新トークン (PRT) を保持しているか確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b53fc-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="b53fc-109">PRT の詳細については、この[ドキュメント](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="b53fc-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="b53fc-110">Azure AD PRT を保持しているか確認するには、デバイスで `dsregcmd/status` コマンドを実行し、“AzureAdPrt” が “YES” であるかを確認します。</span><span class="sxs-lookup"><span data-stu-id="b53fc-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="b53fc-111">"AzureAdPrt" が "NO" の場合は、次を確認してください。</span><span class="sxs-lookup"><span data-stu-id="b53fc-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="b53fc-112">**AD FS でフェデレーション環境を構築しており、ユーザーの家庭のネットワークからは AD FS へアクセスできない場合**: この場合は、"usernamemixed" エンドポイントがエクストラネットからアクセス可能であることを確認します。</span><span class="sxs-lookup"><span data-stu-id="b53fc-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="b53fc-113">AD FS へのアクセスが VPN 越しである場合は、ユーザーが VPN に接続していることを確認し、デバイスに再ログインします。</span><span class="sxs-lookup"><span data-stu-id="b53fc-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="b53fc-114">詳細については、この[ドキュメント](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="b53fc-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="b53fc-115">**デバイスの TPM に問題があり、デバイスを認証できない場合**: "tpm.msc" を実行し、TPM の状態が "準備完了" かどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="b53fc-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="b53fc-116">それ以外の場合は、`dsregcmd/leave` を実行し、デバイスを Azure AD に再び参加させます。</span><span class="sxs-lookup"><span data-stu-id="b53fc-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="b53fc-117">その後、もう一度お試しください。</span><span class="sxs-lookup"><span data-stu-id="b53fc-117">Then, try again.</span></span> <span data-ttu-id="b53fc-118">詳細については、この[ドキュメント](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="b53fc-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="b53fc-119">**サードパーティ ID プロバイダーを使用しているが、これが WS-Trust プロトコル プロバイダーをサポートしていない場合**。</span><span class="sxs-lookup"><span data-stu-id="b53fc-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="b53fc-120">ドキュメントに記載されているとおり、Hybrid Azure AD Join を使用したデバイスは、この場合は動作しません。</span><span class="sxs-lookup"><span data-stu-id="b53fc-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="b53fc-121">サポートが必要な場合は、ID プロバイダーにお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="b53fc-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="b53fc-122">**ユーザーが Windows 10 Accounts なしで Chrome ブラウザーを使用している**、または **Chrome 用の Office 拡張機能を AAD Join を使用したデバイスまたは Hybrid AAD Join を使用したデバイスで PRT を自動的に使用しない**: デバイスベースの条件付きアクセス ポリシーが失敗し、“未登録のデバイス” エラー メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="b53fc-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="b53fc-123">Chrome ブラウザーを正しく使用するには、SCCM または Intune 経由で "Windows 10 Accounts" または "ユーザーの Chrome ブラウザーに Office 拡張機能" をインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="b53fc-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="b53fc-124">詳細については、この[ドキュメント](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="b53fc-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="b53fc-125">拡張機能をリモートでプッシュできない場合は、上記の拡張機能のいずれかを手動でインストールし、デバイスベースの条件付きアクセスの背後にあるアプリケーションにアクセスするようにユーザーに通知します。</span><span class="sxs-lookup"><span data-stu-id="b53fc-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="b53fc-126">詳細については、この[ドキュメント](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="b53fc-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="b53fc-127">**デバイスは正しく Hybrid Azure AD Join を使用するようになったが、Azure AD Connect または Azure portal での変更の同期で誤って削除または無効化された**: この場合は、デバイスで "AzureAdJoined" と "PRT" の状態が有効と表示された場合でも、デバイス オブジェクトは完全に参加したデバイスとして認識されなくなります。</span><span class="sxs-lookup"><span data-stu-id="b53fc-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="b53fc-128">この問題を解決するには、影響を受けたデバイスで `dsregcmd/leave` を実行し、Azure AD にもう一度参加してください。</span><span class="sxs-lookup"><span data-stu-id="b53fc-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="b53fc-129">詳細については、この[ドキュメント](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="b53fc-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="b53fc-130">Windows 10、1809 更新プログラムで VPN またはクラウド プロキシを使用しているデバイスで、"AzureAdPrt" の状態に関する問題、または SSO を使用するアプリの問題 (PRT があるにもかかわらず、Outlook がメールボックスに接続しない場合) が発生する場合は、このパッチ [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) または 4 月の累積更新プログラム [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) を適用して、これらのマシンで PRT 障害が発生しないようにします。</span><span class="sxs-lookup"><span data-stu-id="b53fc-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















