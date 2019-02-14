---
title: SpamHaus によってブロックされたメールの送信エラー
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 249f16d057b0539d71dc514ac35df28ab78fa061
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "29912353"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>メール送信エラー: クライアント ホストが Spamhaus を使用してブロックされました

メッセージを送信した IP アドレスは、[Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245) が所有するブロック リストにあります。Spamhaus によってブロックされる理由には、アカウントが侵害された、パブリック IP アドレスを共有しているコンピューターが侵害された、およびインターネット サービス プロバイダー (ISP) のポリシーが含まれます。考えられる解決策は次のとおりです。
  
- ソース メール サーバーを制御する Office 365 への受信メッセージがブロックされる場合は、原因を特定し、Spamhaus Web サイトからブロックを除去する必要があります。
    
- ソース IP アドレスが他のユーザーに属している Office 365 への受信メッセージがブロックされる場合は、アドレスの所有者が Spamhaus Web サイトからブロックを除去する必要があります。IP アドレスがポリシー ブロック リスト (PBL) にある場合は、所有者が別の静的 IP アドレスを割り当てるか、PBL からアドレスを削除することができます。
    
- Office 365 ドメインからの送信メッセージがブロックされる場合は、そのメッセージがサード パーティ サービス経由でルーティングされる場合にこのエラーを受信することがあります。ブロックされている IP アドレスの所有者を検索するには、WHOIS ルックアップ ツールを使用できます。
    

