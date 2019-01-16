---
title: 既定値を追加することはできません 2010 の承認ワークフロー
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28297115"
---
# <a name="cant-add-default-2010-approval-workflow"></a><span data-ttu-id="0d806-102">既定値を追加することはできません 2010 の承認ワークフロー</span><span class="sxs-lookup"><span data-stu-id="0d806-102">Can't add default 2010 Approval Workflow</span></span>

<span data-ttu-id="0d806-103">、Microsoft SharePoint サイト コレクション内 (「承認の SharePoint 2010」) などのグローバルに再利用可能なワークフローをリストまたはライブラリに追加できません。</span><span class="sxs-lookup"><span data-stu-id="0d806-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="0d806-104">この問題を解決するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="0d806-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="0d806-105">SharePoint Designer 2013 では、サイト コレクションのルート web サイトを開きます。</span><span class="sxs-lookup"><span data-stu-id="0d806-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="0d806-106">[**サイト オブジェクト**] の [**ワークフロー**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="0d806-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="0d806-107">[**ワークフロー** ] リボンの [**新規作成**] セクションでは、**再利用可能なワークフロー**を選択します。</span><span class="sxs-lookup"><span data-stu-id="0d806-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="0d806-p101">**再利用可能なワークフローの作成**フォームで、名前を入力してください \* **Repair2010\*\*\*。**プラットフォームの種類\*\*には、 **SharePoint 2010 ワークフロー**を選択し、 **[ok]** を選択し、します。</span><span class="sxs-lookup"><span data-stu-id="0d806-p101">On the **Create Reusable Workflow** form, enter the name  \* **Repair2010**\* . For **Platform Type**, select **SharePoint 2010 Workflow**, and then select **OK**.</span></span> 
  
5. <span data-ttu-id="0d806-110">[**ワークフロー** ] リボンの [**保存**] セクションでは、**発行**を選択します。</span><span class="sxs-lookup"><span data-stu-id="0d806-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
6. <span data-ttu-id="0d806-p102">[**ワークフロー** ] リボンの [**管理**] セクションで、**グローバルに公開**を選択します。表示される [確認] ダイアログ ボックスで **[ok]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="0d806-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
7. <span data-ttu-id="0d806-p103">Web ブラウザーで、サイト コレクションのルート web サイトを検索し、**サイトの設定**にアクセスし、 \> **サイト コレクションの機能**です。次に、**ワークフロー**機能を切り替えます。</span><span class="sxs-lookup"><span data-stu-id="0d806-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="0d806-115">·フィーチャーが*アクティブ化*の場合は、**非アクティブ化**をクリックし**をアクティブにする**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="0d806-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="0d806-116">·*Deactivated*の機能が表示された場合は、**アクティブ化**をクリックします。</span><span class="sxs-lookup"><span data-stu-id="0d806-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="0d806-117">詳細については、次の[資料](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0d806-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

