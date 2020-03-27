---
title: DLP 問題についての詳細情報
ms.author: pebaum
author: pebaum
manager: laurawi
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2447"
- "3200001"
ms.openlocfilehash: 6525cee0555f1ae67b7d4e32445b9a1537d4a804
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932699"
---
# <a name="information-about-dlp-issues"></a><span data-ttu-id="be9d8-102">DLP 問題に関する情報</span><span class="sxs-lookup"><span data-stu-id="be9d8-102">Information about DLP issues</span></span>

<span data-ttu-id="be9d8-103">**重要**: 多くの SharePoint Online および OneDrive をご利用のお客様は、バックグラウンドで実行されるサービスに対してビジネスに不可欠なアプリケーションを実行します。</span><span class="sxs-lookup"><span data-stu-id="be9d8-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="be9d8-104">これには、コンテンツの移行、データ損失防止 (DLP)、およびバックアップ ソリューションが含まれます。</span><span class="sxs-lookup"><span data-stu-id="be9d8-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="be9d8-105">これらの前例のない時期に、リモート作業シナリオでこれまで以上にサービスに依存しているユーザーに対して、SharePoint Online および OneDrive サービスの可用性と信頼性を確保するための措置を講じています。</span><span class="sxs-lookup"><span data-stu-id="be9d8-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="be9d8-106">この目的をサポートするため、平日の昼間の時間帯に、バックグラウンド アプリ (移行、DLP、およびバックアップ ソリューション) の調整制限を強化しました。</span><span class="sxs-lookup"><span data-stu-id="be9d8-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="be9d8-107">これらのアプリのスループットは、これらの期間では非常に制限されています。</span><span class="sxs-lookup"><span data-stu-id="be9d8-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="be9d8-108">ただし、同地域の夕方および週末には、サービスはバックグラウンド アプリからの非常に大量のリクエストを処理する準備が整います。</span><span class="sxs-lookup"><span data-stu-id="be9d8-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="be9d8-109">**DLP ポリシーに関する情報**</span><span class="sxs-lookup"><span data-stu-id="be9d8-109">**Information on DLP policy**</span></span>

<span data-ttu-id="be9d8-110">データ損失防止 (DLP) ポリシーを使用すると、Office 365 内の機密情報を識別、監視し、自動的に保護できます。</span><span class="sxs-lookup"><span data-stu-id="be9d8-110">With a DLP policy, you can identify, monitor, and automatically protect sensitive information across Office 365.</span></span>

<span data-ttu-id="be9d8-111">詳細については、次のリンク先を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be9d8-111">Please visit these links for more information:</span></span>

- [<span data-ttu-id="be9d8-112">データ損失防止の概要</span><span class="sxs-lookup"><span data-stu-id="be9d8-112">Overview of data loss prevention</span></span>](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies)
- [<span data-ttu-id="be9d8-113">機密情報の種類で検索される情報</span><span class="sxs-lookup"><span data-stu-id="be9d8-113">What the sensitive information types look for</span></span>](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
- [<span data-ttu-id="be9d8-114">カスタムの機密情報の種類を作成する</span><span class="sxs-lookup"><span data-stu-id="be9d8-114">Create a custom sensitive information type</span></span>](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)
- [<span data-ttu-id="be9d8-115">メール通知を送信し、ポリシー ヒントを表示する</span><span class="sxs-lookup"><span data-stu-id="be9d8-115">Send email notifications and show policy tips</span></span>](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
- [<span data-ttu-id="be9d8-116">保持ラベルと DLP により SharePoint Online ファイルを保護する</span><span class="sxs-lookup"><span data-stu-id="be9d8-116">Protect SharePoint Online files with retention labels and DLP</span></span>](https://docs.microsoft.com/office365/securitycompliance/protect-sharepoint-online-files-with-office-365-labels-and-dlp)
- [<span data-ttu-id="be9d8-117">DLP と Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="be9d8-117">DLP and Microsoft Teams</span></span>](https://docs.microsoft.com/office365/securitycompliance/dlp-microsoft-teams)

<span data-ttu-id="be9d8-118">組み込みやカスタムの機密情報の種類を使用してデータをテストするには、**[分類]** > **[機密情報の種類]** で **[テストの種類]** オプションを使用します。</span><span class="sxs-lookup"><span data-stu-id="be9d8-118">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="be9d8-119">詳細については、「[カスタムの機密情報の種類をテストする](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="be9d8-119">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>