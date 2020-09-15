---
title: OneDrive のクラッシュのトラブルシューティング
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665003"
---
# <a name="troubleshoot-onedrive-crashes"></a>OneDrive のクラッシュのトラブルシューティング

OneDrive が繰り返しクラッシュする場合は、次のトラブルシューティングの手順を試してください。

**レジストリ キーが設定されていないことを確認する:**

1. レジストリ エディターを使用して、HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive に移動する
2. DisableFileSyncNGSC が存在し、1 に設定されている場合は、キーを開き、値を 0 に変更します。
3. スタートに移動して手動で OneDrive を起動する ![Windows キーを押し、](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)検索ボックスに「OneDrive」と入力して、「OneDrive」デスクトップ アプリをクリックします。

**OneDrive をリセットする:**

注:

- OneDrive をリセットすると、(設定されている場合は個人の OneDrive を含む) 既存のすべての同期接続が解除されます。
- お使いのコンピューターで OneDrive をリセットしても、ファイルやデータが失われることはありません。

**OneDrive をリセットするには:**

1. Windows キーと R キーを押し、[実行] ダイアログを開きます。
2. 「%localappdata%\Microsoft\OneDrive\onedrive.exe /reset 」と入力し、[OK] を押します。 すぐにコマンド ウィンドウが表示されます。
3. スタートに移動して手動で OneDrive を起動する ![Windows キーを押し、](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)検索ボックスに「OneDrive」と入力して、「OneDrive」デスクトップ アプリをクリックします。

注:

- リセット前にいくつかのフォルダーのみを同期するように選択した場合、同期の完了後、それを再実行する必要があります。 詳細については、「 [コンピューターと同期する OneDrive フォルダーを選択する](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) 」を参照してください。
- 個人用の OneDrive と OneDrive for Business の場合は、これを完了する必要があります。