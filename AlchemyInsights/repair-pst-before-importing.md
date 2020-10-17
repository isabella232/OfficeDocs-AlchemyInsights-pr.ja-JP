---
title: インポート前に .pst ファイルを修復する
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1226"
- "1800027"
ms.assetid: ''
ms.openlocfilehash: 1ed37192a6b054b745fd48fbc01a6b00fa7074ed
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799101"
---
# <a name="repair-pst-file-before-importing"></a>インポート前に .pst ファイルを修復する

.pst ファイルを Outlook にインポートする前に、以下の手順に従いファイルを修復して、ファイルが破損していないことを確認してください。

1. Outlook を終了します。

2. Office プログラム フォルダー (C:\Program Files (x86)\Microsoft Office\root\Office\<Version\> または C:\Program Files\Microsoft Office\root\Office\<Version\>) にある `Scanpst.exe` を検索して実行します。

3. **Microsoft Outlook 受信トレイ修復ツール**で、**[参照]** をクリックして .pst ファイルを検索します (たとえば、C:\Users\\<username\>\AppData\Local\Microsoft\Outlook)。 .pst ファイルを選択し、**[開く]** をクリックします。

4. **[開始]** をクリックしてスキャンを開始します。

5. ファイルにエラーが見つかった場合は、**[修復]** をクリックし、修復が完了したら **[OK]** をクリックします。

6. .pst ファイルを Outlook にもう一度インポートしてみてください。

詳細については、[「Outlook データ ファイルを修復する」](https://support.office.com/article/25663bc3-11ec-4412-86c4-60458afc5253)および[「Outlook .pst ファイルのインポートに関する問題を解決する」](https://support.office.com/article/2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)を参照してください。
