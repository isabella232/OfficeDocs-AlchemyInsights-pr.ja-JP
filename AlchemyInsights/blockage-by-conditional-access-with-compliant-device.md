---
title: 準拠デバイスで条件付きアクセスによりブロックされる
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2021
ms.locfileid: "51038259"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a><span data-ttu-id="b9729-102">準拠デバイスで条件付きアクセスによりブロックされる</span><span class="sxs-lookup"><span data-stu-id="b9729-102">I’m getting blocked by Conditional Access with compliant device</span></span>

<span data-ttu-id="b9729-103">**強くお勧めするツール**</span><span class="sxs-lookup"><span data-stu-id="b9729-103">**Highly Recommended Tools**</span></span>

- <span data-ttu-id="b9729-104">[デバイス登録トラブルシューティング ツール](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - 最も一般的なデバイス登録の問題に関するトラブルシューティングに役立つ包括的なツールです。</span><span class="sxs-lookup"><span data-stu-id="b9729-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - A comprehensive tool that helps troubleshoot the most common device registration issues.</span></span>
- <span data-ttu-id="b9729-105">[テスト デバイス登録接続スクリプト](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - デバイスがシステム アカウントでデバイス登録エンドポイントにアクセスできるようにするために使用されるツールです。</span><span class="sxs-lookup"><span data-stu-id="b9729-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - A tool used to ensure that a device can access Device Registration endpoints under the system account.</span></span>
- <span data-ttu-id="b9729-106">[Azure AD デバイス クリーンアップ スクリプト](https://github.com/mzmaili/AzureADDeviceCleanup) - お使いの環境で古いデバイスを探して管理するために使用されるツールです。</span><span class="sxs-lookup"><span data-stu-id="b9729-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - A tool used to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="b9729-107">準拠デバイスで条件付きアクセスが失敗する理由、または組織のリソースへのサインイン要求中にユーザーが 「**ここからアクセスすることはできません**」というメッセージを受信する場合の一般的な理由を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b9729-107">Here are some common reasons why Conditional Access may be failing for a compliant device or why your users may be receiving **You can't get there from here** message during a sign-in request to an organizational resource.</span></span>

1. <span data-ttu-id="b9729-108">**デバイスが MDM で要求されるデバイスの状態を満たしていない**。</span><span class="sxs-lookup"><span data-stu-id="b9729-108">**Device is not in a required device state with an MDM**:</span></span>

<span data-ttu-id="b9729-109">デバイスが Intune などの承認済みの MDM プロバイダーに登録されており、*準拠デバイスとしてマークされている* ことを確認します。</span><span class="sxs-lookup"><span data-stu-id="b9729-109">Validate that the device is enrolled with an approved MDM provider like Intune and *marked as compliant*.</span></span> <span data-ttu-id="b9729-110">Intune の詳細については、この[ドキュメント](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="b9729-110">For more information on Intune see this [document](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment).</span></span> <span data-ttu-id="b9729-111">デバイスのコンプライアンスと Intune についてさらに理解するには、「[コンプライアンス ポリシーを使用して、Intune で管理するデバイスのルールを設定する](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b9729-111">For better understanding of device compliance and Intune, see [use compliance policy to set rules for devices you manage with Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started).</span></span> <span data-ttu-id="b9729-112">Intune でのデバイスの登録で問題が発生する場合は、「[Microsoft へのデバイス登録のトラブルシューティング](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)」からトラブルシューティングの詳細を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b9729-112">If you are having issues enrolling a device with Intune, find troubleshooting details at [Troubleshoot device enrollment in Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span> <span data-ttu-id="b9729-113">Intune のサポートをさらに希望する場合は、サポート リクエストを作成します。</span><span class="sxs-lookup"><span data-stu-id="b9729-113">For further Intune support, create a support request.</span></span> <span data-ttu-id="b9729-114">この操作を行うには、[[Intune のヘルプ とサポートのページ](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport)] にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="b9729-114">To do so, visit the [Intune Help and Support page](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).</span></span>

2. <span data-ttu-id="b9729-115">**デバイスが組織のネットワークに参加していません**:</span><span class="sxs-lookup"><span data-stu-id="b9729-115">**Device is not joined to the organizations network**:</span></span>

<span data-ttu-id="b9729-116">組織のリソースにアクセスするには、デバイスを組織のネットワークに直接接続するか、仮想プライベート ネットワーク (VPN) を使用して接続し、オンプレミスまたは Azure Active Directory に参加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b9729-116">For access to organizational resources, the device has to be connected to the organization's network, either through direct connection or a virtual private network (VPN), and also joined to on-premise or Azure Active Directory.</span></span> <span data-ttu-id="b9729-117">組織のネットワークに作業デバイスを参加させるには、「[作業デバイスを組織のネットワークに参加させる](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b9729-117">To join a work device to the organization network, see [Join your work device to your organization's network](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network).</span></span> <span data-ttu-id="b9729-118">個人用/BYOD デバイスを登録するには、「[組織のネットワークに個人用デバイスを登録する](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b9729-118">To register a personal/BYOD device, see [Register your personal device on your organization's network](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).</span></span>

- <span data-ttu-id="b9729-119">デバイスがネットワークに参加しているかどうかを検証するには、[ここ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered)から登録済みのデバイスの手順を実行するか、[ ここ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined)から作業デバイスの手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="b9729-119">To validate whether the device has joined the network, you can follow the steps for registered devices [here](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) or work devices [here](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined).</span></span> <span data-ttu-id="b9729-120">問題の範囲を組織のネットワーク接続に指定するには、以下のガイドラインに従ってください。</span><span class="sxs-lookup"><span data-stu-id="b9729-120">To scope the issue to Org network connectivity, follow guidelines below:</span></span>

    1. <span data-ttu-id="b9729-121">職場または学校のアカウント (alain@contoso.com など) を使用して Windows にサインインします。</span><span class="sxs-lookup"><span data-stu-id="b9729-121">Sign in to Windows using your work or school account,  for example, alain@contoso.com.</span></span>
    2. <span data-ttu-id="b9729-122">VPN または DirectAccess を使って組織のネットワークに接続します。</span><span class="sxs-lookup"><span data-stu-id="b9729-122">Connect to your organization's network through a VPN or DirectAccess.</span></span>
    3. <span data-ttu-id="b9729-123">接続した後、**Windows ロゴ キー + L** を押してデバイスをロックします。</span><span class="sxs-lookup"><span data-stu-id="b9729-123">After you're connected, press the **Windows logo key+L** to lock your device.</span></span>
    4. <span data-ttu-id="b9729-124">仕事用または学校用のアカウントを使用してデバイスのロックを解除し、問題のあるアプリまたはサービスにもう一度アクセスしてみます。</span><span class="sxs-lookup"><span data-stu-id="b9729-124">Unlock your device using your work or school account, and then try to access the problematic app or service again.</span></span>

<span data-ttu-id="b9729-125">"**ここからアクセスすることはできません**" というエラー メッセージが再び表示される場合は、他の場所に問題がある可能性があります。</span><span class="sxs-lookup"><span data-stu-id="b9729-125">If you see the **You can't get there from here** error message again, issue is likely elsewhere.</span></span>

3. <span data-ttu-id="b9729-126">**オペレーティング システムはサポートされていません**:</span><span class="sxs-lookup"><span data-stu-id="b9729-126">**Operating system is not supported**:</span></span>

<span data-ttu-id="b9729-127">次に記載するものを含む、サポートされているバージョンのオペレーティング システムを実行していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="b9729-127">Ensure that you're running a supported version of the operating system, including:</span></span>

- <span data-ttu-id="b9729-128">**Windows クライアント**: Windows 7 以降</span><span class="sxs-lookup"><span data-stu-id="b9729-128">**Windows Client**: Windows 7 or later</span></span>

- <span data-ttu-id="b9729-129">**Windows Server**: Windows Server 2008 R2 以降</span><span class="sxs-lookup"><span data-stu-id="b9729-129">**Windows Server**: Windows Server 2008 R2 or later</span></span>

- <span data-ttu-id="b9729-130">**macOS**: macOS X 以降</span><span class="sxs-lookup"><span data-stu-id="b9729-130">**macOS**: macOS X or later</span></span>

- <span data-ttu-id="b9729-131">**Android および iOS**: Android および iOS モバイル オペレーティング システムの最新バージョン</span><span class="sxs-lookup"><span data-stu-id="b9729-131">**Android and iOS**: Latest version of Android and iOS mobile operating systems</span></span>

4. <span data-ttu-id="b9729-132">**Web ブラウザはサポートされていません**。</span><span class="sxs-lookup"><span data-stu-id="b9729-132">**Web browser is not supported**:</span></span>

<span data-ttu-id="b9729-133">以下のサポートされているブラウザーを検索してください。</span><span class="sxs-lookup"><span data-stu-id="b9729-133">Please find supported browsers below.</span></span> <span data-ttu-id="b9729-134">Windows 1703 以降のバージョンでの Chrome のサポートでは、Windows 10 アカウント拡張機能が必要です。</span><span class="sxs-lookup"><span data-stu-id="b9729-134">For Chrome support with Windows 1703 or later versions, a Windows 10 Accounts extension is required.</span></span> <span data-ttu-id="b9729-135">Microsoft Edge 85+ の場合、デバイスのコンプライアンス情報を適切に渡すには、ユーザーがサインインしている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b9729-135">For Edge 85+, the user needs to be signed in to properly pass device compliance information.</span></span> <span data-ttu-id="b9729-136">詳細については、[こちら](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b9729-136">For more details, see [here](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

- <span data-ttu-id="b9729-137">**Windows 10** Microsoft Edge、Internet Explorer、Chrome</span><span class="sxs-lookup"><span data-stu-id="b9729-137">**Windows 10**: Microsoft Edge, Internet Explorer, Chrome</span></span>
- <span data-ttu-id="b9729-138">**Windows 8 / 8.1**: Internet Explorer、 Chrome</span><span class="sxs-lookup"><span data-stu-id="b9729-138">**Windows 8 / 8.1**: Internet Explorer, Chrome</span></span>
- <span data-ttu-id="b9729-139">**Windows 7**: Internet Explorer、 Chrome</span><span class="sxs-lookup"><span data-stu-id="b9729-139">**Windows 7**: Internet Explorer, Chrome</span></span>
- <span data-ttu-id="b9729-140">**iOS**: Microsoft Edge、Intune Managed Browser、Safari</span><span class="sxs-lookup"><span data-stu-id="b9729-140">**iOS**: Microsoft Edge, Intune Managed Browser, Safari</span></span>
- <span data-ttu-id="b9729-141">**Android**: **Microsoft Edge**: Intune Managed Browser、Chrome</span><span class="sxs-lookup"><span data-stu-id="b9729-141">**Android**: **Microsoft Edge**: Intune Managed Browser, Chrome</span></span>
- <span data-ttu-id="b9729-142">**Windows Phone**: Microsoft Edge、Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="b9729-142">**Windows Phone**: Microsoft Edge, Internet Explorer</span></span>
- <span data-ttu-id="b9729-143">**Windows Server 2019**: Microsoft Edge、Internet Explorer、Chrome</span><span class="sxs-lookup"><span data-stu-id="b9729-143">**Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome</span></span>
- <span data-ttu-id="b9729-144">**Windows Server 2016**: Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="b9729-144">**Windows Server 2016**: Internet Explorer</span></span>
- <span data-ttu-id="b9729-145">**Windows Server 2012 R2**: Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="b9729-145">**Windows Server 2012 R2**: Internet Explorer</span></span>
- <span data-ttu-id="b9729-146">**Windows Server 2008 R2**: Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="b9729-146">**Windows Server 2008 R2**: Internet Explorer</span></span>
- <span data-ttu-id="b9729-147">**macOS**: Chrome、Safari</span><span class="sxs-lookup"><span data-stu-id="b9729-147">**macOS**: Chrome, Safari</span></span>

<span data-ttu-id="b9729-148">「**そこにはアクセスできません**」というメッセージとトラブルシューティングの手順の詳細については、[こちら](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b9729-148">Find more information on the **You can't get there** message and troubleshooting steps [here](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation).</span></span>
