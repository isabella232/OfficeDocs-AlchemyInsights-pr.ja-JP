---
title: SharePoint Online のサイトを作成する
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770428"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="5cd20-102">テンプレートを使用して SharePoint サイトを作成する</span><span class="sxs-lookup"><span data-stu-id="5cd20-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="5cd20-103">サイトをテンプレートとして保存する機能は、最新のコミュニケーション サイトまたはチーム サイトではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5cd20-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="5cd20-104">テンプレートの使用の詳細については、「[SharePoint サイトをテンプレートとして保存、ダウンロード、およびアップロードする](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5cd20-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="5cd20-105">これは、SharePoint Online でサイトまたはリストをテンプレートとして保存することに関する一般的な問題 / 解決策です。</span><span class="sxs-lookup"><span data-stu-id="5cd20-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="5cd20-106">**[テンプレートとしてサイト/リストを保存] ボタンが利用できないか、見つからない**</span><span class="sxs-lookup"><span data-stu-id="5cd20-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="5cd20-107">管理者は、テンプレート機能を有効にするためにカスタム スクリプトを許可する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5cd20-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="5cd20-108">詳細な手順、例、および考慮事項については、次を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5cd20-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="5cd20-109">カスタム スクリプトを許可または禁止する</span><span class="sxs-lookup"><span data-stu-id="5cd20-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="5cd20-110">[テンプレートとしてサイトを保存] コマンドはサポートされていないため、SharePoint Server 発行インフラストラクチャを使用するサイトで問題が発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="5cd20-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="5cd20-111">**サイト テンプレートを作成できない、またはサイト テンプレートが正常に機能しない**</span><span class="sxs-lookup"><span data-stu-id="5cd20-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="5cd20-112">テンプレートに[機能](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx)が設定されていないため、有効になりません。</span><span class="sxs-lookup"><span data-stu-id="5cd20-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="5cd20-113">現在のサイト コレクションで機能を有効にできない場合は、サイト テンプレートを使用してサイトを作成することはできません。</span><span class="sxs-lookup"><span data-stu-id="5cd20-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="5cd20-114">サイト テンプレートの作成がブロックされる可能性があるため、リストまたはライブラリが[リスト ビューのしきい値](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59)の5000項目を超えていないかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="5cd20-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="5cd20-115">サイトが多すぎるリソースを使用している可能性があり、サイト テンプレートが50 MB の制限を超えています。</span><span class="sxs-lookup"><span data-stu-id="5cd20-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="5cd20-116">ルックアップ列を使用するリストのデータを表示する際に問題が発生します。</span><span class="sxs-lookup"><span data-stu-id="5cd20-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="5cd20-117">詳細については、「[SharePoint Online で、テンプレートから作成したリストに正しいルックアップ リスト データが表示されない](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5cd20-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="5cd20-118">共通の問題と解決策の詳細については、 「[サイト テンプレートを作成して使用する](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5cd20-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



