---
title: Microsoft Edge で Azure 機能が正常に機能しない場合の対処方法
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584200"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Microsoft Edge で Azure 機能が正常に機能しない場合の対処方法

Microsoft Edge には、セキュリティ ゾーンに関連する[既知の問題](https://go.microsoft.com/fwlink/?linkid=2140608)があり、Azure ユーザーが Windows Admin Center にログインする方法に影響を与える可能性があります。 Microsoft Edge で Azure 機能を使用する際に問題が発生した場合は、次の手順を試してください。

1. **[スタート]** メニューで、**[インターネット オプション]** を検索して選択します。
2. **[プロパティ]** ダイアログ ボックスで **[セキュリティ]** タブに移動します。
3. **[信頼済みサイト]** ゾーンを選択してから、**[サイト]** ボタンを選択します。
4. **[信頼済みサイト]** ダイアログ ボックスで、ゲートウェイ URL と [https://login.microsoftonline.com](https://login.microsoftonline.com) および [https://login.live.com](https://login.live.com) を追加し、**[閉じる]** を選択します。
5. **[インターネット プロパティ]** ダイアログ ボックスで、**[プライバシー]** タブをクリックします。
6. **[ポップアップ ブロック]** セクションで、**[設定]** を選択します。 表示されたダイアログ ボックスで、ゲートウェイ URL と [https://login.microsoftonline.com](https://login.microsoftonline.com) および [https://login.live.com](https://login.live.com) を追加し、**[閉じる]** を選択します。
