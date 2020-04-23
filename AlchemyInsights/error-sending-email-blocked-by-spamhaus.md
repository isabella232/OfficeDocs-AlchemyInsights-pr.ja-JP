---
title: SpamHaus によってブロックされたメールの送信エラー
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714263"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>メール送信エラー: クライアント ホストが Spamhaus を使用してブロックされました

メッセージを送信した IP アドレスは、[Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245) が所有するブロック リストにあります。Spamhaus によってブロックされる理由には、アカウントが侵害された、パブリック IP アドレスを共有しているコンピューターが侵害された、およびインターネット サービス プロバイダー (ISP) のポリシーが含まれます。考えられる解決策は次のとおりです。
  
- 送信元電子メールサーバーを制御するブロックされた受信メッセージの場合は、原因を特定し、Spamhaus web サイトからブロックを削除する必要があります。

- 送信元 IP アドレスが他のユーザーに属しているブロックされた受信メッセージの場合、アドレス所有者は Spamhaus web サイトからそのブロックを削除する必要があります。IP アドレスがポリシーブロック一覧 (PBL) にある場合、所有者は別の静的 IP アドレスを割り当てるか、PBL からアドレスを削除することができます。

- Microsoft に接続されているドメインからのブロックされた送信メッセージの場合、メッセージがサードパーティのサービスを経由してルーティングされると、このエラーが発生することがあります。WHOIS 参照ツールを使用して、ブロックされた IP アドレスの所有者を検索できます。
