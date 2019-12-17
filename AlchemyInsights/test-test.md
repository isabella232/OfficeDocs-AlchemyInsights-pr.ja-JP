---
title: SharePoint Online 用語ストアで用語が見つからない
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053518"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="1ae1b-102">Intune で Bitlocker 暗号化を有効にする</span><span class="sxs-lookup"><span data-stu-id="1ae1b-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="1ae1b-103">Intune のエンドポイント保護ポリシーは、「Intune を使用してデバイスを保護するための Windows 10 (以降) の設定」に記載されているように、Windows デバイスの Boitlocker 暗号化の設定を構成するために使用できます</span><span class="sxs-lookup"><span data-stu-id="1ae1b-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="1ae1b-104">Windows 10 を実行する多くの新しいデバイスでは、MDM ポリシーの適用なしでトリガーされる自動 Boitlocker 暗号化をサポートしていることを、ユーザーは認識する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1ae1b-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="1ae1b-105">これは、非既定の設定が構成されている場合、ポリシーの適用に影響を与える可能性があります。</span><span class="sxs-lookup"><span data-stu-id="1ae1b-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="1ae1b-106">詳細については、FAQ を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1ae1b-106">See FAQ for more detail.</span></span>


<span data-ttu-id="1ae1b-107">FAQ  Q: エンドポイント保護ポリシーを使用するデバイスの暗号化をサポートする Windows のエディションはどれですか?</span><span class="sxs-lookup"><span data-stu-id="1ae1b-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="1ae1b-108"> A: Intune エンドポイント保護ポリシーの設定は、Bitlocker CSP を使用して実装されています。</span><span class="sxs-lookup"><span data-stu-id="1ae1b-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="1ae1b-109">すべての Windows のエディションやビルドで Bitlocker CSP をサポートしているわけではありません。 
     </span><span class="sxs-lookup"><span data-stu-id="1ae1b-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="1ae1b-110">現時点の Windows エディション: Enterprise、Education、Mobile、Mobile Enterprise および Professional (ビルド 1809 以降) がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="1ae1b-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="1ae1b-111">Q: デバイスが、暗号化方法と暗号強度 (XTS-AES-128)  に対する OS の既定の設定を使用している Bitlocker で暗号化されている場合、新しい設定を使用してドライブの再暗号化を自動でトリガーできる、設定の異なるポリシーを適用することはできますか?</span><span class="sxs-lookup"><span data-stu-id="1ae1b-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="1ae1b-112">A: いいえ。</span><span class="sxs-lookup"><span data-stu-id="1ae1b-112">A: No.</span></span> <span data-ttu-id="1ae1b-113">新しい暗号の設定を適用するために、ドライブの暗号化を最初に解除する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1ae1b-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="1ae1b-114">注: OOBE 中に行われる Autopilot の自動暗号化を使用してデバイスが登録されている場合は、OS の既定値の代わりに使用されるポリシー ベースの設定を許可する Intune ポリシーが評価されるまで、トリガーされません。</span><span class="sxs-lookup"><span data-stu-id="1ae1b-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="1ae1b-115">Q: Intune ポリシーを適用した結果としてデバイスが暗号化されている場合、そのポリシーが削除されれば、デバイスの暗号は解除されますか?</span><span class="sxs-lookup"><span data-stu-id="1ae1b-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="1ae1b-116">A: 暗号化関連のポリシーを削除しても、構成されたドライブの暗号は解除されません。</span><span class="sxs-lookup"><span data-stu-id="1ae1b-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="1ae1b-117">Q: Intune コンプライアンス ポリシーで、デバイスは "Bitlocker 有効" な状態ではありませんと表示されるのはどうしてですか?</span><span class="sxs-lookup"><span data-stu-id="1ae1b-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="1ae1b-118">A: Intune コンプライアンス ポリシーの "Bitlocker 有効" の設定では、 Windows デバイス正常性構成証明 (DHA) のクライアントを利用します。</span><span class="sxs-lookup"><span data-stu-id="1ae1b-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="1ae1b-119">このクライアントは、ブート時のデバイスの状態のみ評価します。</span><span class="sxs-lookup"><span data-stu-id="1ae1b-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="1ae1b-120">そのため、Bitlocker 暗号化が完了してからデバイスが再起動されていない場合、DHA クライアント サービスでは Bitlocker をアクティブな状態として報告しません。</span><span class="sxs-lookup"><span data-stu-id="1ae1b-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>