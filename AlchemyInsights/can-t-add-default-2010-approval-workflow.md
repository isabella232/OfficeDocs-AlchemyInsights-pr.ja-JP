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
# <a name="cant-add-default-2010-approval-workflow"></a>既定値を追加することはできません 2010 の承認ワークフロー

、Microsoft SharePoint サイト コレクション内 (「承認の SharePoint 2010」) などのグローバルに再利用可能なワークフローをリストまたはライブラリに追加できません。
  
この問題を解決するには、次の手順を実行します。 
  
1. SharePoint Designer 2013 では、サイト コレクションのルート web サイトを開きます。
  
2. [**サイト オブジェクト**] の [**ワークフロー**] を選択します。 
  
3. [**ワークフロー** ] リボンの [**新規作成**] セクションでは、**再利用可能なワークフロー**を選択します。 
  
4. **再利用可能なワークフローの作成**フォームで、名前を入力してください * **Repair2010***。**プラットフォームの種類**には、 **SharePoint 2010 ワークフロー**を選択し、 **[ok]** を選択し、します。 
  
5. [**ワークフロー** ] リボンの [**保存**] セクションでは、**発行**を選択します。 
  
6. [**ワークフロー** ] リボンの [**管理**] セクションで、**グローバルに公開**を選択します。表示される [確認] ダイアログ ボックスで **[ok]** を選択します。 
  
7. Web ブラウザーで、サイト コレクションのルート web サイトを検索し、**サイトの設定**にアクセスし、 \> **サイト コレクションの機能**です。次に、**ワークフロー**機能を切り替えます。 
  
·フィーチャーが*アクティブ化*の場合は、**非アクティブ化**をクリックし**をアクティブにする**] をクリックします。 
  
·*Deactivated*の機能が表示された場合は、**アクティブ化**をクリックします。 
  
詳細については、次の[資料](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)を参照してください。
  

