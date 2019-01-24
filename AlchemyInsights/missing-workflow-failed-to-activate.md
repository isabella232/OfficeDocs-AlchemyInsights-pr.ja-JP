---
title: ワークフローがありませんを有効にできませんでした。
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 33b92c2cae1f641b0cd88c82fd4ae5e8632d76c2
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29476567"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="9a0ca-102">ワークフローがありませんを有効にできませんでした。</span><span class="sxs-lookup"><span data-stu-id="9a0ca-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="9a0ca-103">、Microsoft SharePoint サイト コレクション内 (「承認の SharePoint 2010」) などのグローバルに再利用可能なワークフローをリストまたはライブラリに追加できません。</span><span class="sxs-lookup"><span data-stu-id="9a0ca-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="9a0ca-104">この問題を解決するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="9a0ca-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="9a0ca-105">SharePoint Designer 2013 では、サイト コレクションのルート web サイトを開きます。</span><span class="sxs-lookup"><span data-stu-id="9a0ca-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="9a0ca-106">[**サイト オブジェクト**] の [**ワークフロー**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="9a0ca-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="9a0ca-107">[**ワークフロー** ] リボンの [**新規作成**] セクションでは、**再利用可能なワークフロー**を選択します。</span><span class="sxs-lookup"><span data-stu-id="9a0ca-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="9a0ca-p101">**再利用可能なワークフローの作成**フォームで、名前を入力してください \* \* *Repair2010* \* \* です。**プラットフォームの種類**には、 **SharePoint 2010 のワークフロー**をクリックし、し、[ **OK**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="9a0ca-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="9a0ca-110">[**ワークフロー** ] リボンの [**保存**] セクションでは、**発行**を選択します。</span><span class="sxs-lookup"><span data-stu-id="9a0ca-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="9a0ca-p102">[**ワークフロー** ] リボンの [**管理**] セクションで、**グローバルに公開**を選択します。表示される [確認] ダイアログ ボックスで **[ok]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="9a0ca-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="9a0ca-p103">Web ブラウザーで、サイト コレクションのルート web サイトを検索し、**サイトの設定**にアクセスし、 \> **サイト コレクションの機能**です。次に、**ワークフロー**機能を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="9a0ca-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="9a0ca-115">·フィーチャーが*アクティブ化*の場合は、**非アクティブ化**をクリックし**をアクティブにする**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="9a0ca-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="9a0ca-116">·*Deactivated*の機能が表示された場合は、**アクティブ化**をクリックします。</span><span class="sxs-lookup"><span data-stu-id="9a0ca-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="9a0ca-117">詳細については、次の[資料](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a0ca-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

