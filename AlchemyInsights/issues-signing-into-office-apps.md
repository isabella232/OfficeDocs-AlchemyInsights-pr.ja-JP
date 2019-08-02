---
title: Office アプリへのサインインの問題
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "36051956"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Office アプリを修正する "コンピューターのトラステッドプラットフォームモジュールが正しく機能していません。" というメッセージが表示される

このエラーを解決するには、次の操作を行います。

- [Windows](https://support.microsoft.com/help/4027667/windows-10-update)および[Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)の最新の更新プログラムをインストールします。
- Windows 資格情報マネージャーを使用して[Office 資格情報をクリア](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)します。<br/>
    **注:** Office 2016 のレジストリパスは16.0 に変更されました。 (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- [ユーザー回復プロセス](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2)を試行して、トラステッドプラットフォームモジュール (TPM) の障害を修正します。
- 次の手順を使用して、EnableADAL = 0 を設定します。  
    1. Windows の [スタート] ボタンを右クリックし、[**実行**] を選択し、「 **regedit**」と入力して、[ **OK]** を選択します。
    2. [**はい]** を選択して、レジストリエディターでデバイスを変更できるようにします。
    3. レジストリエディターで、HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity. の下に**0**の設定を使用して**EnableADAL**の DWORD 値を追加します。

詳細については、「 [Windows 10 の Office 2016 ビルド16.0.7967 での更新後のサインインの接続の問題](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)」を参照してください。