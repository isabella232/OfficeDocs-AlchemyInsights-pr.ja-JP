---
title: ライセンス認証が失敗したワークフローが表示されない
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
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29476567"
---
# <a name="missing-workflow-failed-to-activate"></a>ライセンス認証が失敗したワークフローが表示されない

Microsoft SharePoint サイト コレクションにおいて、グローバルに再利用可能なワークフロー (“承認 - SharePoint 2010” など) をリストまたはライブラリに追加することができません。
  
この問題を解決するには、以下の手順を実行します。 
  
1. SharePoint Designer 2013 で、該当のサイト コレクションのルート Web サイトを開きます。
  
2. [**サイト オブジェクト**] で、[**ワークフロー**] を選択します。 
  
3. [**ワークフロー**] リボンの [**新規作成**] セクションで、[**再利用可能なワークフロー**] を選択します。 
  
4. [**再利用可能なワークフローの作成**] フォームで、名前 ***Repair2010*** を入力します。[**プラットフォームの種類**] で [**SharePoint 2010 ワークフロー**] をクリックし、[**OK**] をクリックします。 
  
1. [**ワークフロー**] リボンの [**保存**] セクションで、[**発行**] を選択します。 
  
2. [**ワークフロー**] リボンの [**管理**] セクションで、[**グローバルに発行**] を選択します。表示される確認ダイアログ ボックスで [**OK**] を選択します。 
  
3. Web ブラウザーで、サイト コレクションのルート Web サイトを見つけて、[**サイトの設定**]、[**サイト コレクションの機能**] の順にアクセスします。次に、**ワークフロー**機能を切り替えます。 
  
本機能が*アクティブ化*されている場合は、[**非アクティブ化**] をクリックしてから、[**アクティブ化**] をクリックします。 
  
本機能が*非アクティブ化*されている場合は、[**アクティブ化**] をクリックします。 
  
詳細については、以下の[記事](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)を参照してください。
  

