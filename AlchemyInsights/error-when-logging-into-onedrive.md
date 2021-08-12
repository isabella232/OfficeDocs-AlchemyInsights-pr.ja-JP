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
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946584"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>OneDrive の起動時に 0x8004de40 エラーが発生する

OneDrive にログインしたときにエラー **0x8004de40** を受け取った場合は、職場または学校のドメインに接続した状態でコンピューターを再起動してください。 再起動後にこのエラーが発生した場合は、職場または学校のドメインに接続しているときにこれを試してください。

1. [スタート] をクリックし、検索ボックスに **cmd** または **コマンド プロンプト** と入力し、コマンド プロンプト アプリを右クリックして、**[管理者として実行する]** を選択します。 管理者のパスワードを要求するダイアログ ボックスが表示された場合はパスワードを入力して [OK] をクリックし、確認を要求するダイアログ ボックスが表示された場合は [**許可**] をクリックします。  

2. コマンド プロンプト ウィンドウで、**dsregcmd /leave** と入力し、コマンドが完了するのを待ちます。 次に、**dsregcmd /join** と入力し、コマンドが完了するのを待ちます。
3. コンピューターを再起動します。
