---
title: 'チームのサインインエラーの対処: AADSTS9000411'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 883bf48d3628702c92361a5250f0d59e1352918349b8bc6c3eae5a948b72fc57
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53953035"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a>チームのサインインエラーの対処: AADSTS9000411

Microsoft Teams にサインインすると、次のエラーが表示されることがあります。 **"申し訳ございませんが、AADSTS9000411 でのサインインで問題が発生しています。要求の形式が正しくありません。パラメーター 「login_hint」 が重複しています。"**

この問題に対処するには、Microsoft Teams クライアントが更新されていることをご確認ください。 クライアントの更新の詳細については、 「[Microsoft Teams の更新プログラム](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)」を参照してください。

何らかの理由でクライアントを更新できない場合、クライアントをログオフすると、キャッシュされているほとんどのデータがクリアされます。 ただし、ログオフ/ログオン後も問題が解決しない場合は、Teams を終了し、次の操作を行って、クライアント キャッシュをクリアします。
1. Microsoft Teams を終了します。
2. %appdata%\microsoft\teams に移動し、すべてのファイルを削除します。
3. Microsoft Teams をもう一度開きます。
