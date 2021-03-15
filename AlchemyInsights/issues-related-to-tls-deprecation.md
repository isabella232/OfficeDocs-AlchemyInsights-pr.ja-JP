---
title: TLS 1.0 および TLS 1.1 の無効化のため、Office 365 でメールを送受信できない
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751149"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>TLS 1.0 および TLS 1.1 の無効化のため、Office 365 でメールを送受信できない

メッセージ センターの投稿 MC229914 で確認された、TLS 1.0 と TLS 1.1 の廃止が Exchange Online のメール フロー エンドポイントへの適用を開始しました。 まもなく、Office 365 は外部ソースからの TLS 1.0 と TLS 1.1 メール接続を受け入れなくなります。 また、Exchange Online は TLS 1.0 または 1.1 を使用してメールを送信することはなくなります。 TLS 1.0 または 1.1 の無効化による問題が発生している場合は、次のいずれかのエラーが発生する可能性があります。

- 送信者が NDR バウンス バックを受信している - '421 4.4.2 SocketError により接続がドロップされました'
- Officer 365 - '421 4.4.2 SocketError により接続がドロップされたオンプレミス サーバーのキュー ビューアーのエラー'
- Office 365 にメールを送信するサーバーのコネクタ [プロトコル ログ](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging)の送信エラー: TLS ネゴシエーションが SocketError エラーによって失敗しました
- コネクタ プロトコル ログの送受信のエラー - '451 5.7.3 最初に STARTTLS コマンドを発行する必要があります'

上記のエラーが発生した場合は、メールの送受信サーバーで TLS 1.2 が有効になっているかどうかを、次のレジストリ キーから確認します。

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**

TLS 1.2 を有効にするために上記のレジストリ キーを変更した場合は、サーバーを再起動して変更を有効にします。 また、最新の Windows と Exchange の更新プログラムがインストールされていることも確認します。

詳細については、以下を参照してください。

- [Exchange Server TLS ガイダンス、パート 1: TLS 1.2 の準備 - Microsoft 技術コミュニティ](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange サーバー TLS ガイダンス パート 2: TLS 1.2 を有効にして、それを使用していないクライアントを特定する - Microsoft 技術コミュニティ](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [TLS バージョンが Exchange Online で合意できない場合のメール シナリオを理解する - Microsoft 技術コミュニティ](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
