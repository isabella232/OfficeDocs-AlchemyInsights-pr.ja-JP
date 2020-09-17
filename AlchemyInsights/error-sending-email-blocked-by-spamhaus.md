---
title: SpamHaus によってブロックされたメールの送信エラー
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783808"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="4d66f-102">メール送信エラー: クライアント ホストが Spamhaus を使用してブロックされました</span><span class="sxs-lookup"><span data-stu-id="4d66f-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="4d66f-p101">メッセージを送信した IP アドレスは、[Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245) が所有するブロック リストにあります。Spamhaus によってブロックされる理由には、アカウントが侵害された、パブリック IP アドレスを共有しているコンピューターが侵害された、およびインターネット サービス プロバイダー (ISP) のポリシーが含まれます。考えられる解決策は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="4d66f-p101">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies. Possible fixes are:</span></span>
  
- <span data-ttu-id="4d66f-106">ソース メール サーバーを制御する受信メッセージがブロックされる場合は、原因を特定し、Spamhaus Web サイトからブロックを除去する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4d66f-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="4d66f-p102">ソース IP アドレスが他のユーザーに属している受信メッセージがブロックされる場合は、アドレスの所有者が Spamhaus Web サイトからブロックを除去する必要があります。IP アドレスがポリシー ブロック リスト (PBL) にある場合は、所有者が別の静的 IP アドレスを割り当てるか、PBL からアドレスを削除することができます。</span><span class="sxs-lookup"><span data-stu-id="4d66f-p102">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website. If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="4d66f-p103">Microsoft に接続されているドメインからの送信メッセージがブロックされる場合は、そのメッセージがサード パーティ サービス経由でルーティングされる場合にこのエラーを受信することがあります。ブロックされている IP アドレスの所有者を検索するには、WHOIS ルックアップ ツールを使用できます。</span><span class="sxs-lookup"><span data-stu-id="4d66f-p103">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service. You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
