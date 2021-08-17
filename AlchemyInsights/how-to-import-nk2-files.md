---
title: how-to-import-nk2-files
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: f2b034926ec165b819119b5c4e060f10022d6017ec5dba8794d18ee3e96c709a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54043211"
---
# <a name="how-to-import-nk2-files"></a>.nk2 ファイルのインポート方法 

ユーザーが初めて Microsoft Outlook 2013、Outlook 2016、Outlook 2019 または Outlook for Microsoft 365 を使用するときに、ユーザーのニックネーム キャッシュ (*profilename*.nk2 ファイルに保存されています) が既定のメッセージ ストアの非表示メッセージにインポートされます。

.nk2 ファイルを Outlook 2013、Outlook 2016、Outlook 2019 または Outlook for Microsoft 365 にインポートするために、.nk2 ファイルがフォルダー %appdata%\Microsoft\Outlook にあることを確認してください。

**注**: .nk2 ファイルの名前は、現在の Outlook 2013 または Outlook 2016 プロファイルと同じ名前にする必要があります。 既定では、このプロファイルの名前は "Outlook" です。 プロファイルの名前を確認するには、次の手順を実行します。 
1. **[スタート]** ボタンをクリックし、**[コントロール パネル]** をクリックします。
2. **[メール]** をダブルクリックします。
3. [メール設定] ダイアログ ボックスで、**[プロファイルの表示]** を選択します。
4. **[開始]** > **[実行]** をクリックします。
5. **[開く]** ボックスで、「*outlook.exe /importnk2*」と入力して **[OK]** をクリックします。 

.nk2 ファイルをインポートすると、そのファイルの内容はメールボックスに保存されている既存のニックネーム キャッシュに結合されます。

**注**: .nk2 ファイルの名前は、Outlook 2013、Outlook 2016、Outlook 2019 または Outlook for Microsoft 365 の次回起動時に .old というファイル拡張子付きに変更されます。 .nk2 ファイルを再インポートする場合は、最初にファイル拡張子 .old を削除してください。

詳細については、「[オートコンプリートのリストを別のコンピューターにインポートまたはコピーする](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)」を参照してください。