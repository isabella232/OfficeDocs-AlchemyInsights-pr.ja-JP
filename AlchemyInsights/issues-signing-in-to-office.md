---
title: Office アプリへのサインインに関する問題
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
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "36051955"
---
# <a name="blank-sign-in-screen-in-office-apps"></a>Office アプリでの空のサインイン画面

この問題を解決するには、次の操作を試してください。
- [Windows](https://support.microsoft.com/help/4027667/windows-10-update) および [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5) の最新の更新プログラムをインストールします。
- Internet Explorer のオプションをリセットする: [**ツール**]  >  [**インターネット オプション**]  >  [**詳細設定**]  >  [**Internet Explorer の設定をリセット**] の順に移動します (ユーザー設定が失われることにご留意ください)。その後、Office にもう一度サインインしてみてください。
- Windows Defender Application Guard (WDAG) または同様のファイアウォールやウイルス対策ソフトウェアを無効にします。
    1. [コントロール パネル] で [**プログラム**] に移動し、[**Windows の機能の有効化または無効化**] を選択します。
    2. Windows Defender Application Guard が有効になっている場合は、無効にしてみてください。<br/>
    **注:** コンピューターの再起動が必要な場合があります。
- Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) がアプリケーション、ファイアウォール、ウイルス対策プログラムによってブロックされていないことを確認します。
- Windows 資格情報マネージャーを使用して、[Office の資格情報をクリア](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)します。<br/>
    **注:** Office 2016 のレジストリ パスは 16.0 に変更されています。 (例: \Software\Microsoft\Office\16.0\Common\Identity\)

詳細については、「[Windows 10 の Office 2016 ビルド16.0.7967 に更新後のサインインにおける接続の問題](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)」を参照してください。