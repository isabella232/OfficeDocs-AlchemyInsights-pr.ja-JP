---
title: DLP が期待どおりに機能していない
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e96904e2f0da2fe1fafb3f8722465eaf22681b71
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507483"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="910e6-102">DLP が期待どおりに機能していない</span><span class="sxs-lookup"><span data-stu-id="910e6-102">DLP not working as expected</span></span>

<span data-ttu-id="910e6-103">**重要**: これらの前例のない時期にも、SharePoint Online および OneDrive サービスの可用性を維持するための措置を講じています。詳細については、「[SharePoint Online の一時的な機能調整](https://aka.ms/ODSPAdjustments)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="910e6-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="910e6-104">**DLP のセットアップ**</span><span class="sxs-lookup"><span data-stu-id="910e6-104">**Setting up DLP**</span></span>

<span data-ttu-id="910e6-105">Office 365の**データ損失防止 (DLP)** で問題が発生していませんか？</span><span class="sxs-lookup"><span data-stu-id="910e6-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="910e6-106">その場合は、**DLPポリシー**が正しく設定されていること、およびデータに**DLPポリシー**が評価のさいに探しているものが含まれていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="910e6-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="910e6-107">DLP policies allows you to identify and protect sensitive information in your organization.</span><span class="sxs-lookup"><span data-stu-id="910e6-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="910e6-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="910e6-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="910e6-109">**DLP ポリシーの検索基準**</span><span class="sxs-lookup"><span data-stu-id="910e6-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="910e6-110">セキュリティ/コンプライアンス センターで**組み込みの機密情報の種類**を使用する場合、これらの機密の種類を検出するときに、DLP ポリシーでは特定のパターンと要素が検索されます。</span><span class="sxs-lookup"><span data-stu-id="910e6-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="910e6-111">**組み込みの機密情報の種類**</span><span class="sxs-lookup"><span data-stu-id="910e6-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="910e6-112">組み込みの機密の種類の詳細および機密の種類を検出するときに DLP ポリシーで検索される内容については、「[機密情報の種類の検索基準](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="910e6-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="910e6-113">**カスタムの機密情報の種類**</span><span class="sxs-lookup"><span data-stu-id="910e6-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="910e6-114">カスタムの機密情報の種類を作成する場合、カスタムの機密の種類の作成方法については、「[カスタムの機密情報の種類を作成する](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)」の記事を使用してください。</span><span class="sxs-lookup"><span data-stu-id="910e6-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="910e6-115">**DLP ポリシーをテストする**</span><span class="sxs-lookup"><span data-stu-id="910e6-115">**Test a DLP policy**</span></span>

<span data-ttu-id="910e6-116">組み込みやカスタムの機密情報の種類を使用してデータをテストするには、**[分類]** > **[機密情報の種類]** で **[テストの種類]** オプションを使用します。</span><span class="sxs-lookup"><span data-stu-id="910e6-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="910e6-117">詳細については、「[カスタムの機密情報の種類をテストする](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="910e6-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="910e6-118">**レポート**</span><span class="sxs-lookup"><span data-stu-id="910e6-118">**Reports**</span></span>
  
- <span data-ttu-id="910e6-119">[DLP レポート](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)で機密データの分析情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="910e6-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="910e6-120">[インシデント レポート](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)でイベントの特定の詳細を確認します。</span><span class="sxs-lookup"><span data-stu-id="910e6-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
