---
title: 2010 の承認ワークフローを追加できない
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: e74c842f8b4be321664f8c2f1f58c570d0724d80edb1264add0647bf313bc82f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020341"
---
# <a name="unable-to-add-2010-approval-workflow"></a>2010 の承認ワークフローを追加できない

Microsoft SharePoint サイト コレクションにおいて、グローバルに再利用可能なワークフロー (“承認 - SharePoint 2010” など) をリストまたはライブラリに追加できません。
  
この問題を解決するには、次の手順を実行します。 
  
1. SharePoint Designer 2013 で、該当のサイト コレクションのルート Web サイトを開きます。
  
2. **[サイト オブジェクト]** で、**[ワークフロー]** を選択します。 
  
3. [**ワークフロー**] リボンの [**新規作成**] セクションで、[**再利用可能なワークフロー**] を選択します。 
  
4. [**再利用可能なワークフローの作成**] フォームで、名前 ***Repair2010*** を入力します。[**プラットフォームの種類**] で [**SharePoint 2010 ワークフロー**] をクリックし、[**OK**] をクリックします。 
  
1. [**ワークフロー**] リボンの [**保存**] セクションで、[**発行**] を選択します。 
  
2. [**ワークフロー**] リボンの [**管理**] セクションで、[**グローバルに発行**] を選択します。表示される確認ダイアログ ボックスで [**OK**] を選択します。 
  
3. Web ブラウザーで、サイト コレクションのルート Web サイトを見つけて、[**サイトの設定**]、[**サイト コレクションの機能**] の順にアクセスします。**ワークフロー** 機能を次のように切り替えます。 
  
本機能が *アクティブ化* されている場合は、[**非アクティブ化**] をクリックしてから、[**アクティブ化**] をクリックします。 
  
本機能が *非アクティブ化* されている場合は、**[アクティブ化]** をクリックします。 
  
詳細については、次の[記事](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)を参照してください。
  

