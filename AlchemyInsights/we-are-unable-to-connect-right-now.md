---
title: ライセンス承認の問題 - 現在接続できない
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
- "3408"
- "9001423"
ms.openlocfilehash: 5dad4b43efac2468b57351a4d6c96379ed505071ca144ec0aa518e975633bb18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998160"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Microsoft 365 アプリの「現在接続できません」メッセージを修正

このメッセージが表示された場合は、次を試してください。

1. ファイアウォール、ウイルス対策ソフトウェア、プロキシ設定を確認し、インターネットが Microsoft 365 アプリにアクセスするのをそれらがブロックしていないことを確認します。 「[Microsoft の URL と IP アドレスの範囲](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)」を参照してください。

2. [**開始**] > [**実行**] に移動して、**services.msc** と入力します。 次のサービスがすべて実行されていることを確認してください。
    - ネットワーク接続デバイスの自動セットアップ
    - ネットワーク リスト サービス
    - ネットワーク上の場所の認知
    - Windows イベント ログ

これらのサービスのいずれかが実行されていない場合は、開始してみてください。 サービスの開始に問題がある場合は、昇格されたアクセス許可でコマンド プロンプトを開いて次のコマンドを実行します。

**sfc /scannow**

このコマンドが終了したら、コンピューターを再起動します。

詳細については、「[Microsoft 365 から Office のライセンス認証を行う際の "申し訳ありませんが、アカウントに接続できません。しばらくしてからもう一度お試しください"](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)」エラーを参照してください。