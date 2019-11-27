---
title: 2010 の承認ワークフローを追加できない
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 13e3ed6db8c31adb1eb5a556c0e5fbc437b3fdb1
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36748689"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="a20ab-102">2010 の承認ワークフローを追加できない</span><span class="sxs-lookup"><span data-stu-id="a20ab-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="a20ab-103">Microsoft SharePoint サイト コレクションにおいて、グローバルに再利用可能なワークフロー (“承認 - SharePoint 2010” など) をリストまたはライブラリに追加できません。</span><span class="sxs-lookup"><span data-stu-id="a20ab-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="a20ab-104">この問題を解決するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="a20ab-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="a20ab-105">SharePoint Designer 2013 で、該当のサイト コレクションのルート Web サイトを開きます。</span><span class="sxs-lookup"><span data-stu-id="a20ab-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="a20ab-106">**[サイト オブジェクト]** で、**[ワークフロー]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="a20ab-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="a20ab-107">[**ワークフロー**] リボンの [**新規作成**] セクションで、[**再利用可能なワークフロー**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a20ab-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="a20ab-p101">[**再利用可能なワークフローの作成**] フォームで、名前 ***Repair2010*** を入力します。[**プラットフォームの種類**] で [**SharePoint 2010 ワークフロー**] をクリックし、[**OK**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a20ab-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="a20ab-110">[**ワークフロー**] リボンの [**保存**] セクションで、[**発行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a20ab-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="a20ab-p102">[**ワークフロー**] リボンの [**管理**] セクションで、[**グローバルに発行**] を選択します。表示される確認ダイアログ ボックスで [**OK**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a20ab-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="a20ab-p103">Web ブラウザーで、サイト コレクションのルート Web サイトを見つけて、[**サイトの設定**]、[**サイト コレクションの機能**] の順にアクセスします。**ワークフロー**機能を次のように切り替えます。</span><span class="sxs-lookup"><span data-stu-id="a20ab-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="a20ab-115">本機能が*アクティブ化*されている場合は、[**非アクティブ化**] をクリックしてから、[**アクティブ化**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a20ab-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="a20ab-116">本機能が*非アクティブ化*されている場合は、**[アクティブ化]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a20ab-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="a20ab-117">詳細については、次の[記事](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a20ab-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

