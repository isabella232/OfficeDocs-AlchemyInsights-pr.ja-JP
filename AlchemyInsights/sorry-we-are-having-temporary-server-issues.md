---
title: Office アプリの「申し訳ありませんが、一時的なサーバーの問題が発生しています」メッセージの修正
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764122"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Office アプリの「申し訳ありませんが、一時的なサーバーの問題が発生しています」メッセージを修正

このメッセージが表示された場合は、次を試してください。

1. ファイアウォール、ウイルス対策ソフトウェア、プロキシ設定を確認し、インターネットが Office アプリにアクセスするのをそれらがブロックしていないことを確認します。 「 [URL と IP アドレスの範囲](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)」を参照してください。

2. [**開始**] > [**実行**] に移動して、**services.msc** と入力します。 次のサービスがすべて実行されていることを確認してください。
    - ネットワーク接続デバイスの自動セットアップ
    - ネットワーク リスト サービス
    - ネットワーク上の場所の認知
    - Windows イベント ログ

これらのサービスのいずれかが実行されていない場合は、開始してみてください。 サービスの開始に問題がある場合は、昇格されたアクセス許可でコマンド プロンプトを開いて次のコマンドを実行します。

**sfc /scannow**

このコマンドが終了したら、コンピューターを再起動します。

詳細については、「[ライセンス認証を行う際の ”申し訳ありませんが、アカウントに接続できません。しばらくしてからもう一度お試しください”](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)」エラーを参照してください。