---
title: Microsoft 365 アプリへのサインインに関する問題
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
- "9000571"
- "2559"
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986896"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Microsoft 365 アプリでの「このコンピューターのトラステッド プラットフォーム モジュールが正常に機能していません」というメッセージを解決する

このエラーを解決するには、次の操作を行います。

- [Windows](https://support.microsoft.com/help/4027667/windows-10-update) および [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5) の最新の更新プログラムをインストールします。
- Windows 資格情報マネージャーを使用して、[Office の資格情報をクリア](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer)します。<br/>
    **注:** Office 2016 のレジストリ パスは 16.0 に変更されています。(例: \Software\Microsoft\Office\16.0\Common\Identity\)
- [ユーザー回復プロセス](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2)を実行して、トラステッド プラットフォーム モジュール (TPM) の障害の解決を試みてください。
- 次の手順に従い、EnableADAL = 0 に設定します。  
    1. Windows の [スタート] ボタンを右クリックし、[**ファイル名を指定して実行**] を選択します。"**regedit**" と入力し、[**OK**] を選択します。
    2. [**はい**] を選択して、レジストリ エディターがデバイスに変更を加えることを許可します。
    3. レジストリ エディターで、HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity に **EnableADAL** の DWORD 値を **0** に設定して追加します。

詳細については、「[Windows 10 の Office 2016 ビルド16.0.7967 に更新後のサインインにおける接続の問題](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)」を参照してください。