---
title: DataProtection-Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/30/2019
ms.locfileid: "40923551"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="3d43f-102">Intune で Bitlocker 暗号化を有効にする</span><span class="sxs-lookup"><span data-stu-id="3d43f-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="3d43f-103">Intune Endpoint Protection ポリシーを使用して、Windows デバイスの Bitlocker 暗号化設定を構成できます。</span><span class="sxs-lookup"><span data-stu-id="3d43f-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="3d43f-104">詳細については、「 [Windows 10 以降の設定」の「Intune を使用してデバイスを保護する](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3d43f-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="3d43f-105">Windows 10 を実行している新しいデバイスの多くは、自動 Bitlocker 暗号化をサポートしていますが、これは MDM ポリシーの適用なしでトリガーされることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="3d43f-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="3d43f-106">既定以外の設定が構成されている場合、ポリシーの適用に影響する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="3d43f-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="3d43f-107">詳細については、次の FAQ を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3d43f-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="3d43f-108">Bitlocker の問題のトラブルシューティングの詳細については、「 [Microsoft Intune での bitlocker ポリシーのトラブルシューティング](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3d43f-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="3d43f-109">**FAQ**</span><span class="sxs-lookup"><span data-stu-id="3d43f-109">**FAQ**</span></span>

 <span data-ttu-id="3d43f-110">Q: エンドポイント保護ポリシーを使用してデバイスの暗号化をサポートしている Windows のエディションを教えてください。</span><span class="sxs-lookup"><span data-stu-id="3d43f-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="3d43f-111">A: Intune Endpoint Protection ポリシーの設定は、 [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)を使用して実装されています。</span><span class="sxs-lookup"><span data-stu-id="3d43f-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="3d43f-112">Windows のすべてのエディションまたはビルドが Bitlocker CSP をサポートするわけではありません。</span><span class="sxs-lookup"><span data-stu-id="3d43f-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="3d43f-113">現時点では、次の Windows エディションがサポートされています。 Enterprise、エデュケーション、Mobile、Mobile Enterprise、Professional (ビルド1809以降)。</span><span class="sxs-lookup"><span data-stu-id="3d43f-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="3d43f-114">Q: 暗号化方式と暗号強度 (XTS-128) の OS の既定の設定を使用して、デバイスが既に Bitlocker で暗号化されている場合、別の設定のポリシーを適用すると、新しい設定でドライブの再暗号化が自動的にトリガーされますか。</span><span class="sxs-lookup"><span data-stu-id="3d43f-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="3d43f-115">A: いいえ。</span><span class="sxs-lookup"><span data-stu-id="3d43f-115">A: No.</span></span> <span data-ttu-id="3d43f-116">新しい cipher 設定を適用するには、最初にドライブを復号化する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3d43f-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="3d43f-117">**注:** 自動操縦によって登録されているデバイスの場合、OOBE 中に発生する自動暗号化は、Intune ポリシーが評価されるまでトリガーされないため、ポリシーベースの設定を OS の既定値の代わりに使用できます。</span><span class="sxs-lookup"><span data-stu-id="3d43f-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="3d43f-118">Q: Intune ポリシーを適用した結果としてデバイスが暗号化されている場合、そのポリシーが削除されると、暗号化が解除されますか。</span><span class="sxs-lookup"><span data-stu-id="3d43f-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="3d43f-119">A: 暗号化関連のポリシーを削除しても、構成されたドライブの暗号化が解除されることはありません。</span><span class="sxs-lookup"><span data-stu-id="3d43f-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="3d43f-120">Q: Intune コンプライアンスポリシーが、Bitlocker が有効になっていないのに、Bitlocker が有効になっていないことを示しているのはなぜですか?</span><span class="sxs-lookup"><span data-stu-id="3d43f-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="3d43f-121">A: Intune コンプライアンスポリシーの "Bitlocker enabled" 設定は、Windows デバイス正常性構成証明 (DHA) クライアントを利用します。</span><span class="sxs-lookup"><span data-stu-id="3d43f-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="3d43f-122">このクライアントは、ブート時のデバイスの状態のみ評価します。</span><span class="sxs-lookup"><span data-stu-id="3d43f-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="3d43f-123">Bitlocker 暗号化が完了してからデバイスが再起動されていない場合、DHA クライアントサービスは Bitlocker をアクティブとして報告しません。</span><span class="sxs-lookup"><span data-stu-id="3d43f-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 