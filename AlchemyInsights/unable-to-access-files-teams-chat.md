---
title: Teams チャットで共有されているファイルにアクセスできない
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10825"
- "9003042"
ms.openlocfilehash: 42731693c062b961bdd3bf7b728ea64f705765e539ee751903dd57f263d11ae0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54092445"
---
# <a name="unable-to-access-files-shared-in-teams-chat"></a>Teams チャットで共有されているファイルにアクセスできない

Microsoft Teams では、チャット ウィンドウでユーザーが共有したファイルは、共有ユーザーの OneDrive サイトに自動的に保存されます。

他のユーザーが Teams でファイルを開こうとしたときに "このファイルへのアクセス権がありません" というエラー メッセージが表示される場合、この問題は、制限付きアクセス ユーザーのアクセス許可ロックダウン モード機能が OneDrive サイトで有効になっていることが原因で発生しています。

1. OneDrive サイトで機能を無効にする方法については、「[Error when opening a file in Teams (Teams でファイルを開くときのエラー)](https://go.microsoft.com/fwlink/?linkid=2155733)」を参照してください。

1. 他のユーザーが OneDrive サイトへのアクセス権を持っているかどうかを確認し、「[OneDrive のファイルとフォルダーの共有](https://go.microsoft.com/fwlink/?linkid=2156017)」の手順に従ってアクセス権を付与します。