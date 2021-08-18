---
title: Teams が起動しない
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/4/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12673"
- "9007646"
ms.openlocfilehash: ebfabf667092850e5045c56e34e355739944ba44
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329331"
---
# <a name="teams-doesnt-launch"></a>Teams が起動しない

Microsoft Teams を開こうとしても起動しない場合は、次の操作を試してください。

1. **%appdata%\Microsoft\Teams** に移動します。
1. フォルダーの内容を削除します。
1. コンピューターを再起動し、Teams の起動を試行します。

Teams の再インストールが必要になる場合があります。 再インストールするには、次のようにします。

1. [コントロール パネル] を使って Teams をアンインストールします。
1. **%appdata%\Microsoft\Teams\Application Cache** に移動します。
1. フォルダーの内容を削除します。
1. **%appdata%\Microsoft\teams\Cache** に移動します。
1. フォルダーの内容を削除します。
1. コンピューターを再起動し、Teams をダウンロードしてインストールします。

サインインできない特定のユーザーに対してテナントで診断を実行する場合は、**TeamsUserUnableToSignIn** キーワードを使用して新しい検索を開始し、画面の指示に従います。