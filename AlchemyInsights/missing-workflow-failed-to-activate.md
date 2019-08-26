---
title: ライセンス認証が失敗したワークフローが表示されない
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 44fd3c2d1e8b278b47c0fde6d48c7cbcbaa5c324
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543930"
---
# <a name="missing-workflow-failed-to-activate"></a>ライセンス認証が失敗したワークフローが表示されない

Microsoft SharePoint サイト コレクションにおいて、グローバルに再利用可能なワークフロー (“承認 - SharePoint 2010” など) をリストまたはライブラリに追加することができません。
  
この問題を解決するには、次の手順を実行します。 
  
1. SharePoint Designer 2013 で、該当のサイト コレクションのルート Web サイトを開きます。
  
2. **[サイト オブジェクト]** で、**[ワークフロー]** を選択します。 
  
3. [**ワークフロー**] リボンの [**新規作成**] セクションで、[**再利用可能なワークフロー**] を選択します。 
  
4. [**再利用可能なワークフローの作成**] フォームで、名前 ***Repair2010*** を入力します。[**プラットフォームの種類**] で [**SharePoint 2010 ワークフロー**] をクリックし、[**OK**] をクリックします。 
  
1. [**ワークフロー**] リボンの [**保存**] セクションで、[**発行**] を選択します。 
  
2. **[ワークフロー]** リボンの **[管理]** セクションで、**[グローバルに発行]** を選択します。表示される確認ダイアログ ボックスで **[OK]** を選択します。 
  
3. Web ブラウザーで、サイト コレクションのルート Web サイトを見つけて、**[サイトの設定]** \> **[サイト コレクションの機能]** の順にアクセスします。次に、**ワークフロー**機能を切り替えます。 
  
本機能が*アクティブ化*されている場合は、**[非アクティブ化]** をクリックしてから、**[アクティブ化]** をクリックします。 
  
本機能が*非アクティブ化*されている場合は、**[アクティブ化]** をクリックします。 
  
詳細については、次の[記事](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)を参照してください。
  

