---
title: ライセンスの認証/サインインの問題 - トラステッド プラットフォーム モジュールの誤動作
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3406"
- "9001429"
ms.openlocfilehash: d1c25bb283def13524b1dcd19d0c746ee32c4e11
ms.sourcegitcommit: efdde3c24a0c1adfb8b6f5f59dcae435fb5c53a8
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/19/2019
ms.locfileid: "38749429"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Office アプリでの「このコンピューターのトラステッド プラットフォーム モジュールが正常に機能していません 」というメッセージを解決する

このエラーを解決するには、次の操作を行います。

1. Office アプリを開き、すべての既存のユーザー アカウントから[サインアウト](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)します。   
2. Windows を使用して [**設定**] > [**アカウント**] > [**メールとアカウント**] の順に移動し、既存の職場のアカウントを削除します。 
3. Windows を使用して [**設定**] > [**アカウント**] > [**職場または学校にアクセスする**] の順に移動し、既存のアカウントを切断します。 
4. Office のライセンス認証の状態を再設定します。 [詳細情報](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state
)を参照してください。
5. [ユーザー回復プロセス](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2)を実行して、トラステッド プラットフォーム モジュール (TPM) の障害の解決を試みてください。