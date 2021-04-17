---
title: 'AIP: ヘッダーとフッターが期待どおりに表示されない'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4541"
ms.openlocfilehash: 5f50fc1d38618017bca61b4e9290d9893983534e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821704"
---
# <a name="aip-headers-and-footers-not-displaying-as-expected"></a><span data-ttu-id="b7e73-102">AIP: ヘッダーとフッターが期待どおりに表示されない</span><span class="sxs-lookup"><span data-stu-id="b7e73-102">AIP: Headers and footers not displaying as expected</span></span>

<span data-ttu-id="b7e73-103">視覚的なマーキングが期待どおりに表示されない問題が発生している場合は、次のガイドラインを参照してください。</span><span class="sxs-lookup"><span data-stu-id="b7e73-103">If you are experiencing issues with visual markings not displaying as expected, view the following guidelines:</span></span>

1. <span data-ttu-id="b7e73-104">「[視覚的なマーキングが適用される場合](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)」を確認してください。</span><span class="sxs-lookup"><span data-stu-id="b7e73-104">Make sure you have reviewed [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="b7e73-105">Officeのラベル付けについては、「[Office 365 がコンテンツにマーキングと暗号化を適用した場合](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption)」を確認してください。</span><span class="sxs-lookup"><span data-stu-id="b7e73-105">For Office labeling, review [When Office 365 applies content marking and encryption](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption).</span></span>
3. <span data-ttu-id="b7e73-106">既存のヘッダー/フッターを削除する場合は、「[他のラベル付けソリューションからヘッダーとフッターを削除する](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions)」を確認してください。</span><span class="sxs-lookup"><span data-stu-id="b7e73-106">If you want to remove existing headers/footers, review [Remove headers and footers from other labeling solutions](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions).</span></span>

<span data-ttu-id="b7e73-107">それでも問題が発生する場合は、Azure Information Protection クライアント ログを収集し、エクスポートしたログをこのチケットに添付します。</span><span class="sxs-lookup"><span data-stu-id="b7e73-107">If you are still experiencing the issue, collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

<span data-ttu-id="b7e73-108">**Azure Information Protection ログをエクスポートする**</span><span class="sxs-lookup"><span data-stu-id="b7e73-108">**Export Azure Information Protection logs**</span></span>

1. <span data-ttu-id="b7e73-109">Office ドキュメントを開くか、Outlook で新しいメールを作成します。</span><span class="sxs-lookup"><span data-stu-id="b7e73-109">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="b7e73-110">[**保護/感度** > **へルプとフィードバック**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="b7e73-110">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="b7e73-111">[**ログのエクスポート**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="b7e73-111">Click **Export Logs**.</span></span>
4. <span data-ttu-id="b7e73-112">ログを選択した場所に保存し、このサービス要求に添付します。</span><span class="sxs-lookup"><span data-stu-id="b7e73-112">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="b7e73-113">追加情報については、次を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b7e73-113">For additional information, see:</span></span>

- [<span data-ttu-id="b7e73-114">Azure Information Protection 用の視覚的なマーキングのラベルを構成する方法</span><span class="sxs-lookup"><span data-stu-id="b7e73-114">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="b7e73-115">Azure Information Protection のドキュメントを確認する</span><span class="sxs-lookup"><span data-stu-id="b7e73-115">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="b7e73-116">Azure Information Protection の要件</span><span class="sxs-lookup"><span data-stu-id="b7e73-116">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="b7e73-117">Azure Information Protection のクイック スタート チュートリアル</span><span class="sxs-lookup"><span data-stu-id="b7e73-117">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [<span data-ttu-id="b7e73-118">Azure Information Protection クライアントをダウンロードする</span><span class="sxs-lookup"><span data-stu-id="b7e73-118">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
