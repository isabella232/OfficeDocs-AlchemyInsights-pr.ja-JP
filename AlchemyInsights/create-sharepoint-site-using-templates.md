---
title: SharePoint Online のサイトを作成する
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 9ab06cbd1648da31d8a04e61c237a2326b4bbe93
ms.sourcegitcommit: f856d46a325c517fc29d935c27f21b77c4219e66
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/24/2019
ms.locfileid: "35199278"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="46a30-102">テンプレートを使用して SharePoint サイトを作成する</span><span class="sxs-lookup"><span data-stu-id="46a30-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="46a30-103">SharePoint サイト テンプレートは、特定のビジネス ニーズに基づいて設計された作成済みの定義です。</span><span class="sxs-lookup"><span data-stu-id="46a30-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="46a30-104">詳細については、「[テンプレートを使用して、さまざまな種類の SharePoint サイトを作成する](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="46a30-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="46a30-105">ここでは、サイトまたはリストを Sharepoint Online でテンプレートとして保存する場合の一般的な問題と解決策を示します。</span><span class="sxs-lookup"><span data-stu-id="46a30-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="46a30-106">**[サイトの保存/リストテンプレート] ボタンが使用できない、または見つからない**</span><span class="sxs-lookup"><span data-stu-id="46a30-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="46a30-107">管理者は、テンプレート機能を有効にするためにカスタム スクリプトを許可する必要があります。</span><span class="sxs-lookup"><span data-stu-id="46a30-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="46a30-108">詳細な手順については、「例」と「考慮事項」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="46a30-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="46a30-109">カスタム スクリプトを許可または禁止する</span><span class="sxs-lookup"><span data-stu-id="46a30-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="46a30-110">[テンプレートとしてサイトを保存] コマンドはサポートされていないため、SharePoint Server 発行インフラストラクチャを使用するサイトで問題が発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="46a30-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="46a30-111">**サイト テンプレートを作成できないか、正しく機能しない**</span><span class="sxs-lookup"><span data-stu-id="46a30-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="46a30-112">テンプレートが[機能](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx)を持たず、アクティブ化されない場合があります。</span><span class="sxs-lookup"><span data-stu-id="46a30-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="46a30-113">現在のサイト コレクションで機能を有効にできない場合は、サイト テンプレートを使用してサイトを作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="46a30-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="46a30-114">サイト テンプレートの作成がブロックされる可能性があるため、リストまたはライブラリが[リスト ビューのしきい値](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59)の5000項目を超えていないかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="46a30-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="46a30-115">サイトで使用されているリソースが多すぎるため、サイトテンプレートが 50 MB の制限を超えている可能性があります。</span><span class="sxs-lookup"><span data-stu-id="46a30-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="46a30-116">ルックアップ列を使用するリストのデータを表示する際に問題が発生します。</span><span class="sxs-lookup"><span data-stu-id="46a30-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="46a30-117">詳細については、「[テンプレートで生成されるリスト」で、SharePoint Online の適切な参照リストからのデータを表示しません](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a)。</span><span class="sxs-lookup"><span data-stu-id="46a30-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>

<span data-ttu-id="46a30-118">一般的な問題と解決策の詳細については、「[サイトテンプレートを作成して使用する](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="46a30-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



