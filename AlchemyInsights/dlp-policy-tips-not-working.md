---
title: DLP ポリシーのヒントが機能しない
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 8a3b8175c077b77d1c9b5d859012faddcb1fa3a0
ms.sourcegitcommit: 099704f7f4bdf122d09bb4f7cc71d36fc77a7fcf
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2021
ms.locfileid: "51958707"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="70bc3-102">DLP ポリシーのヒントに関する問題</span><span class="sxs-lookup"><span data-stu-id="70bc3-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="70bc3-103">**重要**: これらの前例のない時期にも、SharePoint Online および OneDrive サービスの可用性を維持するための措置を講じています。詳細については、「[SharePoint Online の一時的な機能調整](https://aka.ms/ODSPAdjustments)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="70bc3-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="70bc3-104">セキュリティ/コンプライアンス センターの完全実施モードで DLP ポリシーに関するポリシーのヒントを構成するには、次の手順を実行します：</span><span class="sxs-lookup"><span data-stu-id="70bc3-104">To configure policy tips on your DLP policy in the Security & Compliance center in full enforcement mode, do the following:</span></span>

- <span data-ttu-id="70bc3-105">DLP ルールでポリシー ヒントを **有効** になっていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="70bc3-105">Ensure policy tips have been **enabled** on the DLP rule.</span></span> <span data-ttu-id="70bc3-106">それを確認するには、[メール通知を送信して、DLP ポリシーのヒントを表示する](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="70bc3-106">For steps, see [Send email notifications and show policy tips for DLP policies](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="70bc3-107">コンテンツが、[機密情報の種類エンティティ](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)に略述されているルールをトリガーするために必要な点を満たしていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="70bc3-107">Ensure your content matches what is required to trigger the rule outlined in [Sensitive information type entity definitions](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="70bc3-108">ポリシーのヒントは OWA と Outlook の両方に表示されます。</span><span class="sxs-lookup"><span data-stu-id="70bc3-108">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="70bc3-109">ただし、Outlook 2013 以降をお使いの場合、ポリシー ヒントは特定の条件でのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="70bc3-109">However, when using Outlook 2013 or later, policy tips are displayed only under certain conditions.</span></span> <span data-ttu-id="70bc3-110">特定の条件の一覧については、「[ポリシー ヒントの詳細について Outlook 2013 以降でサポートされている条件を確認する](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="70bc3-110">For the specific conditions list, see [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

<span data-ttu-id="70bc3-111">DLP ポリシー ヒントの詳細については、「[DLP ポリシー ヒント のリファレンス](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps)」 および「[ DLP ポリシー ヒント サポート マトリックス](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="70bc3-111">For information on DLP Policy tips, see [DLP Policy Tips Reference](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) and [Support Matrix for DLP Policy tips](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps).</span></span>