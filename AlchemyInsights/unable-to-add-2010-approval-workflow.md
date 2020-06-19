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
# <a name="unable-to-add-2010-approval-workflow"></a>2010 の承認ワークフローを追加できない

Microsoft SharePoint サイト コレクションにおいて、グローバルに再利用可能なワークフロー (“承認 - SharePoint 2010” など) をリストまたはライブラリに追加できません。
  
この問題を解決するには、次の手順を実行します。 
  
1. SharePoint Designer 2013 で、該当のサイト コレクションのルート Web サイトを開きます。
  
2. **[サイト オブジェクト]** で、**[ワークフロー]** を選択します。 
  
3. [**ワークフロー**] リボンの [**新規作成**] セクションで、[**再利用可能なワークフロー**] を選択します。 
  
4. On the **Create Reusable Workflow** form, enter the name ** *Repair2010* **. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**. 
  
1. [**ワークフロー**] リボンの [**保存**] セクションで、[**発行**] を選択します。 
  
2. In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**. 
  
3. In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Toggle the **Workflows** feature: 
  
本機能が*アクティブ化*されている場合は、[**非アクティブ化**] をクリックしてから、[**アクティブ化**] をクリックします。 
  
本機能が*非アクティブ化*されている場合は、**[アクティブ化]** をクリックします。 
  
詳細については、次の[記事](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)を参照してください。
  

