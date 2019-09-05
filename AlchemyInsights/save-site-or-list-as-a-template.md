---
title: サイトまたはリストをテンプレートとして保存する
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 1fe0a2f5bf65ef4e8cabf3d05a701c8eff966435
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752037"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="99961-102">サイトまたはリストをテンプレートとして保存する</span><span class="sxs-lookup"><span data-stu-id="99961-102">Save site or list as a template</span></span>

<span data-ttu-id="99961-103">SharePoint サイト テンプレートは、特定のビジネス ニーズに基づいて設計された作成済みの定義です。</span><span class="sxs-lookup"><span data-stu-id="99961-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="99961-104">詳細については、「[テンプレートを使用して、さまざまな種類の SharePoint サイトを作成する](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="99961-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="99961-105">これは、SharePoint Online でサイトまたはリストをテンプレートとして保存することに関する一般的な問題/解決策です。</span><span class="sxs-lookup"><span data-stu-id="99961-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="99961-106">**[テンプレートとしてサイト/リストを保存] ボタンが利用できないか、見つからないです**。</span><span class="sxs-lookup"><span data-stu-id="99961-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="99961-107">管理者は、テンプレート機能を有効にするためにカスタム スクリプトを許可する必要があります。</span><span class="sxs-lookup"><span data-stu-id="99961-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="99961-108">詳細な手順、例、および考慮事項については、「[カスタム スクリプトを許可または禁止する](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="99961-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="99961-109">[テンプレートとしてサイトを保存] コマンドはサポートされていないため、SharePoint Server 発行インフラストラクチャを使用するサイトで問題が発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="99961-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="99961-110">**サイト テンプレートを作成できないか、正しく機能しない**</span><span class="sxs-lookup"><span data-stu-id="99961-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="99961-111">テンプレートに[機能](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx)が設定されていないため、有効になりません。</span><span class="sxs-lookup"><span data-stu-id="99961-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="99961-112">現在のサイト コレクションで機能を有効にできない場合は、サイト テンプレートを使用してサイトを作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="99961-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="99961-113">サイト テンプレートの作成がブロックされる可能性があるため、リストまたはライブラリが[リスト ビューのしきい値](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59)の5000項目を超えていないかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="99961-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="99961-114">サイトが多すぎるリソースを使用している可能性があり、サイト テンプレートが50メガバイト (MB) の制限を超えています。</span><span class="sxs-lookup"><span data-stu-id="99961-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="99961-115">ルックアップ列を使用するリストのデータを表示する際に問題が発生します。</span><span class="sxs-lookup"><span data-stu-id="99961-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="99961-116">詳細については、「[SharePoint Online で、テンプレートから作成したリストに正しいルックアップ リスト データが表示されない](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="99961-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="99961-117">共通の問題と解決策の詳細については、 「[サイト テンプレートを作成して使用する](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="99961-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

