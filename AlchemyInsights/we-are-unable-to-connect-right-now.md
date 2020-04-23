---
title: ライセンス承認の問題 - 現在接続できない
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716177"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>Office アプリの「現在接続できません」メッセージを修正

このメッセージが表示された場合は、次を試してください。

1. ファイアウォール、ウイルス対策ソフトウェア、プロキシ設定を確認し、インターネットが Office アプリにアクセスするのをそれらがブロックしていないことを確認します。 「 [Microsoft url と IP アドレスの範囲」を](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)参照してください。

2. [**開始**] > [**実行**] に移動して、**services.msc** と入力します。 次のサービスがすべて実行されていることを確認してください。
    - ネットワーク接続デバイスの自動セットアップ
    - ネットワーク リスト サービス
    - ネットワーク上の場所の認知
    - Windows イベント ログ

これらのサービスのいずれかが実行されていない場合は、開始してみてください。 サービスの開始に問題がある場合は、昇格されたアクセス許可でコマンド プロンプトを開いて次のコマンドを実行します。

**sfc /scannow**

このコマンドが終了したら、コンピューターを再起動します。

詳細については、「[申し訳ございません。アカウントに接続できません。」を参照してください。Microsoft 365 から Office をライセンス認証する際に、後でもう一度実行](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)してください。