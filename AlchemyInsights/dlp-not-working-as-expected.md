---
title: DLP が期待どおりに機能していない
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: db8c6bf7cfb74a85bbbf2992b91a6cb0f233f194
ms.sourcegitcommit: 6c104d686acbce8fa9adeaaedaa44b132b74321a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/29/2019
ms.locfileid: "33470023"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="bb604-102">DLP が期待どおりに機能していない</span><span class="sxs-lookup"><span data-stu-id="bb604-102">DLP not working as expected</span></span>


<span data-ttu-id="bb604-103">Office 365の**データ損失防止 (DLP)** で問題が発生していませんか？</span><span class="sxs-lookup"><span data-stu-id="bb604-103">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="bb604-104">その場合は、**DLPポリシー**が正しく設定されていること、およびデータに**DLPポリシー**が評価のさいに探しているものが含まれていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="bb604-104">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span> 
  
 <span data-ttu-id="bb604-105">**DLP のセットアップ:**</span><span class="sxs-lookup"><span data-stu-id="bb604-105">**Setting up DLP:**</span></span>
  
<span data-ttu-id="bb604-p102">DLP ポリシーによって、組織の機密情報を識別および保護することができます。DLP ポリシーをセットアップするには、[こちら](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)の情報を使用します。</span><span class="sxs-lookup"><span data-stu-id="bb604-p102">DLP policies allows you to identify and protect sensitive information in your organization. To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="bb604-108">**DLP ポリシーの検索基準:**</span><span class="sxs-lookup"><span data-stu-id="bb604-108">**What DLP policies look for:**</span></span>
  
<span data-ttu-id="bb604-109">Office 365 セキュリティ/コンプライアンス センターで**組み込みの機密情報の種類**を使用する場合、これらの機密の種類を検出するときに、DLP ポリシーでは特定のパターンと要素が検索されます。</span><span class="sxs-lookup"><span data-stu-id="bb604-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span> 
  
- <span data-ttu-id="bb604-110">**組み込みの機密情報の種類:**</span><span class="sxs-lookup"><span data-stu-id="bb604-110">**Built-in Sensitive Information Types:**</span></span>
    
    <span data-ttu-id="bb604-111">組み込みの機密の種類の詳細および機密の種類を検出するときに DLP ポリシーで検索される内容については、「[機密情報の種類の検索基準](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb604-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>
    
- <span data-ttu-id="bb604-112">**カスタムの機密情報の種類:**</span><span class="sxs-lookup"><span data-stu-id="bb604-112">**Custom Sensitive Information Types:**</span></span>
    
    <span data-ttu-id="bb604-113">カスタムの機密情報の種類を作成する場合、カスタムの機密の種類の作成方法については、「[カスタムの機密情報の種類を作成する](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)」の記事を使用してください。</span><span class="sxs-lookup"><span data-stu-id="bb604-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>
    
 <span data-ttu-id="bb604-114">**レポート:**</span><span class="sxs-lookup"><span data-stu-id="bb604-114">**Reports:**</span></span>
  
- <span data-ttu-id="bb604-115">[DLP レポート](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)で機密データの分析情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="bb604-115">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>
    
- <span data-ttu-id="bb604-116">[インシデント レポート](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)でイベントの特定の詳細を確認します。</span><span class="sxs-lookup"><span data-stu-id="bb604-116">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
    

