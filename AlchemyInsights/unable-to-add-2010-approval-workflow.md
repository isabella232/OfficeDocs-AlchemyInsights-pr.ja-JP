---
title: 2010 の承認ワークフローを追加できない
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: f40716dd399fe7bea1b606cd725676268dc0a66d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582852"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="3c176-102">2010 の承認ワークフローを追加できない</span><span class="sxs-lookup"><span data-stu-id="3c176-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="3c176-103">Microsoft SharePoint サイト コレクションにおいて、グローバルに再利用可能なワークフロー (“承認 - SharePoint 2010” など) をリストまたはライブラリに追加できません。</span><span class="sxs-lookup"><span data-stu-id="3c176-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="3c176-104">この問題を解決するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="3c176-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="3c176-105">SharePoint Designer 2013 で、該当のサイト コレクションのルート Web サイトを開きます。</span><span class="sxs-lookup"><span data-stu-id="3c176-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="3c176-106">**[サイト オブジェクト]** で、**[ワークフロー]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="3c176-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="3c176-107">[**ワークフロー**] リボンの [**新規作成**] セクションで、[**再利用可能なワークフロー**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3c176-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="3c176-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span><span class="sxs-lookup"><span data-stu-id="3c176-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="3c176-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span><span class="sxs-lookup"><span data-stu-id="3c176-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="3c176-110">[**ワークフロー**] リボンの [**保存**] セクションで、[**発行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3c176-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="3c176-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span><span class="sxs-lookup"><span data-stu-id="3c176-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="3c176-112">In the confirmation dialog box that appears, select **OK**.</span><span class="sxs-lookup"><span data-stu-id="3c176-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="3c176-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span><span class="sxs-lookup"><span data-stu-id="3c176-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="3c176-114">Toggle the **Workflows** feature:</span><span class="sxs-lookup"><span data-stu-id="3c176-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="3c176-115">本機能が*アクティブ化*されている場合は、[**非アクティブ化**] をクリックしてから、[**アクティブ化**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="3c176-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="3c176-116">本機能が*非アクティブ化*されている場合は、**[アクティブ化]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="3c176-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="3c176-117">詳細については、次の[記事](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3c176-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

