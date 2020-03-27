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
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932627"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="ca095-102">DLP が期待どおりに機能していない</span><span class="sxs-lookup"><span data-stu-id="ca095-102">DLP not working as expected</span></span>

<span data-ttu-id="ca095-103">**重要**: 多くの SharePoint Online および OneDrive をご利用のお客様は、バックグラウンドで実行されるサービスに対してビジネスに不可欠なアプリケーションを実行します。</span><span class="sxs-lookup"><span data-stu-id="ca095-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="ca095-104">これには、コンテンツの移行、データ損失防止 (DLP)、およびバックアップ ソリューションが含まれます。</span><span class="sxs-lookup"><span data-stu-id="ca095-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="ca095-105">これらの前例のない時期に、リモート作業シナリオでこれまで以上にサービスに依存しているユーザーに対して、SharePoint Online および OneDrive サービスの可用性と信頼性を確保するための措置を講じています。</span><span class="sxs-lookup"><span data-stu-id="ca095-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="ca095-106">この目的をサポートするため、平日の昼間の時間帯に、バックグラウンド アプリ (移行、DLP、およびバックアップ ソリューション) の調整制限を強化しました。</span><span class="sxs-lookup"><span data-stu-id="ca095-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="ca095-107">これらのアプリのスループットは、これらの期間では非常に制限されています。</span><span class="sxs-lookup"><span data-stu-id="ca095-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="ca095-108">ただし、同地域の夕方および週末には、サービスはバックグラウンド アプリからの非常に大量のリクエストを処理する準備が整います。</span><span class="sxs-lookup"><span data-stu-id="ca095-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

 <span data-ttu-id="ca095-109">**DLP のセットアップ**</span><span class="sxs-lookup"><span data-stu-id="ca095-109">**Setting up DLP**</span></span>

<span data-ttu-id="ca095-110">Office 365の**データ損失防止 (DLP)** で問題が発生していませんか？</span><span class="sxs-lookup"><span data-stu-id="ca095-110">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="ca095-111">その場合は、**DLPポリシー**が正しく設定されていること、およびデータに**DLPポリシー**が評価のさいに探しているものが含まれていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="ca095-111">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="ca095-p104">DLP ポリシーによって、組織の機密情報を識別および保護することができます。DLP ポリシーをセットアップするには、[こちら](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)の情報を使用します。</span><span class="sxs-lookup"><span data-stu-id="ca095-p104">DLP policies allows you to identify and protect sensitive information in your organization. To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="ca095-114">**DLP ポリシーの検索基準**</span><span class="sxs-lookup"><span data-stu-id="ca095-114">**What DLP policies look for**</span></span>
  
<span data-ttu-id="ca095-115">Office 365 セキュリティ/コンプライアンス センターで**組み込みの機密情報の種類**を使用する場合、これらの機密の種類を検出するときに、DLP ポリシーでは特定のパターンと要素が検索されます。</span><span class="sxs-lookup"><span data-stu-id="ca095-115">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="ca095-116">**組み込みの機密情報の種類**</span><span class="sxs-lookup"><span data-stu-id="ca095-116">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="ca095-117">組み込みの機密の種類の詳細および機密の種類を検出するときに DLP ポリシーで検索される内容については、「[機密情報の種類の検索基準](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ca095-117">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="ca095-118">**カスタムの機密情報の種類**</span><span class="sxs-lookup"><span data-stu-id="ca095-118">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="ca095-119">カスタムの機密情報の種類を作成する場合、カスタムの機密の種類の作成方法については、「[カスタムの機密情報の種類を作成する](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)」の記事を使用してください。</span><span class="sxs-lookup"><span data-stu-id="ca095-119">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="ca095-120">**DLP ポリシーをテストする**</span><span class="sxs-lookup"><span data-stu-id="ca095-120">**Test a DLP policy**</span></span>

<span data-ttu-id="ca095-121">組み込みやカスタムの機密情報の種類を使用してデータをテストするには、**[分類]** > **[機密情報の種類]** で **[テストの種類]** オプションを使用します。</span><span class="sxs-lookup"><span data-stu-id="ca095-121">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="ca095-122">詳細については、「[カスタムの機密情報の種類をテストする](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="ca095-122">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="ca095-123">**レポート**</span><span class="sxs-lookup"><span data-stu-id="ca095-123">**Reports**</span></span>
  
- <span data-ttu-id="ca095-124">[DLP レポート](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)で機密データの分析情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="ca095-124">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="ca095-125">[インシデント レポート](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)でイベントの特定の詳細を確認します。</span><span class="sxs-lookup"><span data-stu-id="ca095-125">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
