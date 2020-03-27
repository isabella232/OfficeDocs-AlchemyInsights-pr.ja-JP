---
title: DLP ポリシーのヒントが機能しない
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 6375fa8077529f36ae95d6632ad4d2db5625dc29
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977239"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="f0cf9-102">DLP ポリシーのヒントに関する問題</span><span class="sxs-lookup"><span data-stu-id="f0cf9-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="f0cf9-103">**重要**: これらの従来の状況では、sharepoint Online と OneDrive のサービスの可用性を確保するための手順を実行しています。詳細については、「 [Sharepoint online の一時的な機能の調整](https://aka.ms/ODSPAdjustments)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f0cf9-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="f0cf9-104">**DLP ポリシーヒント**</span><span class="sxs-lookup"><span data-stu-id="f0cf9-104">**DLP policy tips**</span></span>

<span data-ttu-id="f0cf9-105">**DLPポリシー**を使用している場合は、**ポリシーのヒント**を使用してポリシー違反をユーザーに通知できます。</span><span class="sxs-lookup"><span data-stu-id="f0cf9-105">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="f0cf9-106">管理者は、DLPポリシーをテストしている間、ポリシーが完全実施モードになっているときいずれの場合でも表示されるポリシーのヒントを設定できます。</span><span class="sxs-lookup"><span data-stu-id="f0cf9-106">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="f0cf9-107">セキュリティ/コンプライアンス センターの完全実施モードでDLPポリシーに関するポリシーのヒントを構成するには、次の手順を実行します：</span><span class="sxs-lookup"><span data-stu-id="f0cf9-107">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="f0cf9-108">DLP ルールでポリシー ヒントを**有効**にします。そのためには、[こちら](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="f0cf9-108">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="f0cf9-109">**コンテンツが、[こちら](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)の記事に略述されているルールをトリガーする**ために**必要な**点を満たしていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="f0cf9-109">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="f0cf9-p102">ポリシー ヒントは OWA と Outlook の両方に表示されますが、**Outlook 2013 以降**を使用する場合、ポリシー ヒントが表示されるのは特定の条件下に限定されます。該当する条件については、次の資料に記されています: [ポリシー ヒントを表示するために Outlook 2013 以降でサポートされている条件](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="f0cf9-p102">Policy tips display in both OWA and Outlook. However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions. These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="f0cf9-113">DLP ポリシー ヒントについての追加情報については、以下をご覧ください: [DLP ポリシーのポリシー ヒントを表示する](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="f0cf9-113">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  