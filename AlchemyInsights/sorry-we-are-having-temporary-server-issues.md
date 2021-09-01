---
title: Microsoft 365 アプリの「申し訳ありませんが、一時的なサーバーの問題が発生しています」メッセージの修正
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
- "3420"
- "9001430"
ms.openlocfilehash: 565f70d9a09c61bef84cdd1c23e9b0ed34bebe51
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744672"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Microsoft 365 アプリの「申し訳ありませんが、一時的なサーバーの問題が発生しています」メッセージを修正

注: 以前のバージョンの Windows (Windows 7 SP1、Windows Server 2008 R2 など) を使用している場合は、[簡単な修正プログラム](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi)を使用して TLS 1.2 を既定として有効にします。 詳細については、「[Windows の WinHTTP で TLS 1.1 および TLS 1.2 を既定のセキュリティで保護されたプロトコルとして有効にするための更新プログラム](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)」を参照してください。

このメッセージが表示された場合は、次を試してください。

1. ファイアウォール、ウイルス対策ソフトウェア、プロキシ設定を確認し、インターネットが Microsoft 365 アプリにアクセスするのをそれらがブロックしていないことを確認します。 「 [URL と IP アドレスの範囲](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)」を参照してください。

2. [**開始**] > [**実行**] に移動して、**services.msc** と入力します。 次のサービスがすべて実行されていることを確認してください。
    - ネットワーク接続デバイスの自動セットアップ
    - ネットワーク リスト サービス
    - ネットワーク上の場所の認知
    - Windows イベント ログ

これらのサービスのいずれかが実行されていない場合は、開始してみてください。 サービスの開始に問題がある場合は、昇格されたアクセス許可でコマンド プロンプトを開いて次のコマンドを実行します。

**sfc /scannow**

このコマンドが終了したら、コンピューターを再起動します。

詳細については、「[ライセンス認証を行う際の ”申し訳ありませんが、アカウントに接続できません。しばらくしてからもう一度お試しください”](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)」エラーを参照してください。