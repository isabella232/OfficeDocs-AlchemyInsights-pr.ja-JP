---
title: DataProtection - Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 482c08b31e4d97ca5cc9ec6e35e309cb7536036d
ms.sourcegitcommit: 58ac31a58c956a4d74f66bd4151a2311dc361b78
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/07/2021
ms.locfileid: "49778198"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="f77f7-102">Intune で Bitlocker 暗号化を有効にする</span><span class="sxs-lookup"><span data-stu-id="f77f7-102">Enabling Bitlocker encryption with Intune</span></span>

<span data-ttu-id="f77f7-103">Intune エンドポイント保護ポリシーを使用して、Windows デバイスの BitLocker 暗号化設定を構成できます。</span><span class="sxs-lookup"><span data-stu-id="f77f7-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="f77f7-104">詳細については、「[Intune を使用してデバイスを保護する Windows 10 以降の設定](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f77f7-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>

<span data-ttu-id="f77f7-105">エンドポイント保護ポリシーに加えて、デバイスの暗号化状態のより詳細なビューを提供する暗号化レポートもあります。</span><span class="sxs-lookup"><span data-stu-id="f77f7-105">In addition to the Endpoint Protection Policy there is also an Encryption Report which provides a more detailed view of the encryption status for devices.</span></span> <span data-ttu-id="f77f7-106">このレポートには、MEM ポータルの **[デバイス]、[モニター]** からアクセスし、[**構成**] で [[暗号化レポート](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport)] を選択します。</span><span class="sxs-lookup"><span data-stu-id="f77f7-106">This report can be accessed from the MEM portal under **Devices > Monitor**, and then under **Configuration** select [Encryption report](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).</span></span>

<span data-ttu-id="f77f7-107">Bitlocker が期待どおりに有効になっていない場合、または Bitlocker を有効にするために使用されているプロファイルがエラー状態にある場合は、暗号化レポートを確認して、動作が発生している理由をよりよく理解してください。</span><span class="sxs-lookup"><span data-stu-id="f77f7-107">If you find that Bitlocker fails to be enabled as expected or that the profile being used to enable Bitlocker is in an error state, please review the encryption report to get a better understanding of why the behavior is occurring.</span></span>

<span data-ttu-id="f77f7-108">さまざまな暗号化状態の値を含むレポートの解釈方法の詳細については、「[Intune を使用したデバイス暗号化の監視](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f77f7-108">To find details on how to interpret the report including the various encryption status values, see [Monitor device encryption with Intune](https://docs.microsoft.com/mem/intune/protect/encryption-monitor).</span></span>

<span data-ttu-id="f77f7-109">Windows 10 を実行する多くの新しいデバイスでは、MDM ポリシーの適用なしでトリガーされる自動 Bitlocker 暗号化をサポートしていることを、ユーザーは認識する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f77f7-109">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="f77f7-110">これは、非既定の設定が構成されている場合、ポリシーの適用に影響を与える可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f77f7-110">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="f77f7-111">詳細については、次の FAQ を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f77f7-111">See the following FAQ for more detail.</span></span>

<span data-ttu-id="f77f7-112">Bitlocker の問題のトラブルシューティングについては、「[Microsoft Intune の BitLocker ポリシーのトラブルシューティング](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f77f7-112">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="f77f7-113">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="f77f7-113">**FAQ**</span></span>

<span data-ttu-id="f77f7-114">Q: エンドポイント保護ポリシーを使用するデバイスの暗号化をサポートする Windows のエディションはどれですか?</span><span class="sxs-lookup"><span data-stu-id="f77f7-114">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="f77f7-115">A: Intune Endpoint Protectionポリシーの設定は、[Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) を使用して実装されています。</span><span class="sxs-lookup"><span data-stu-id="f77f7-115">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="f77f7-116">すべての Windows のエディションまたはビルドで Bitlocker CSP をサポートしているわけではありません。</span><span class="sxs-lookup"><span data-stu-id="f77f7-116">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="f77f7-117">Q: エンド ユーザーの操作を必要とせずに、デバイスで Bitlocker を有効にするにはどうすればよいですか?</span><span class="sxs-lookup"><span data-stu-id="f77f7-117">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="f77f7-118">A: 必要な前提条件が満たされている限り、Intune を使用して Bitlocker の "Silent Encryption" を有効にできます。</span><span class="sxs-lookup"><span data-stu-id="f77f7-118">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="f77f7-119">デバイス要件およびサイレント暗号化を有効にするためのポリシー設定の例についての詳細は、次のドキュメント: 「[Bitlocker 暗号化を静かに有効化する](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices)」をご参照ください。</span><span class="sxs-lookup"><span data-stu-id="f77f7-119">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="f77f7-120">Q: デバイスが、暗号化方法と暗号強度 (XTS-AES-128) に対する OS の既定の設定を使用している Bitlocker で暗号化されている場合、新しい設定を使用してドライブの再暗号化を自動でトリガーできる、設定の異なるポリシーを適用することはできますか?</span><span class="sxs-lookup"><span data-stu-id="f77f7-120">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="f77f7-121">A: いいえ。</span><span class="sxs-lookup"><span data-stu-id="f77f7-121">A: No.</span></span> <span data-ttu-id="f77f7-122">新しい暗号の設定を適用するには、ドライブの暗号化を最初に解除する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f77f7-122">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="f77f7-123">**注**: OOBE 中に行われる Autopilot の自動暗号化を使用してデバイスが登録されている場合は、OS の既定値の代わりに使用されるポリシー ベースの設定を許可する Intune ポリシーが評価されるまで、トリガーされません。</span><span class="sxs-lookup"><span data-stu-id="f77f7-123">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="f77f7-124">Q: Intune ポリシーを適用した結果としてデバイスが暗号化されている場合、そのポリシーが削除されれば、デバイスの暗号は解除されますか?</span><span class="sxs-lookup"><span data-stu-id="f77f7-124">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="f77f7-125">A: 暗号化関連のポリシーを削除しても、構成されたドライブの暗号は解除されません。</span><span class="sxs-lookup"><span data-stu-id="f77f7-125">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="f77f7-126">Q: Intune コンプライアンス ポリシーで、Bitlocker が有効になっているにもかかわらず有効になっていないと表示されるのはどうしてですか?</span><span class="sxs-lookup"><span data-stu-id="f77f7-126">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="f77f7-127">A: Intune コンプライアンス ポリシーの「Bitlocker 有効」設定では、 Windows デバイス正常性構成証明 (DHA) のクライアントを利用します。</span><span class="sxs-lookup"><span data-stu-id="f77f7-127">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="f77f7-128">このクライアントは、ブート時のデバイスの状態のみ評価します。</span><span class="sxs-lookup"><span data-stu-id="f77f7-128">This client only measures device state at boot time.</span></span> <span data-ttu-id="f77f7-129">そのため、Bitlocker 暗号化が完了してからデバイスが再起動されていない場合、DHA クライアント サービスでは Bitlocker をアクティブな状態として報告しません。</span><span class="sxs-lookup"><span data-stu-id="f77f7-129">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 