---
title: OneDrive の起動時に 0x8004de40 エラーが発生する
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813657"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>OneDrive の起動時に 0x8004de40 エラーが発生する

OneDrive にログインしたときにエラー **0x8004de40** を受け取った場合は、職場または学校のドメインに接続した状態でコンピューターを再起動してください。 再起動後にこのエラーが発生した場合は、職場または学校のドメインに接続しているときにこれを試してください。

1. [スタート] をクリックし、検索ボックスに **cmd** または **コマンド プロンプト** と入力し、コマンド プロンプト アプリを右クリックして、**[管理者として実行する]** を選択します。 管理者のパスワードを要求するダイアログ ボックスが表示された場合はパスワードを入力して [OK] をクリックし、確認を要求するダイアログ ボックスが表示された場合は [**許可**] をクリックします。  

2. コマンド プロンプト ウィンドウで、**dsregcmd /leave** と入力し、コマンドが完了するのを待ちます。 次に、**dsregcmd /join** と入力し、コマンドが完了するのを待ちます。
3. コンピューターを再起動します。
