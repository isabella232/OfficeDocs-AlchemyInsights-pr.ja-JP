---
title: 送信メールが迷惑メール フォルダーへ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 371d2c46e9048365fd343145330536bd9cf1db82
ms.sourcegitcommit: 1002f510fadb92c143cd6bbb60b42a851d5a38e1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/20/2019
ms.locfileid: "37313910"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="77401-102">送信メールが迷惑メール フォルダーへ</span><span class="sxs-lookup"><span data-stu-id="77401-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="77401-103">送信メッセージが迷惑メールとしてマークされている場合には、以下の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="77401-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="77401-104">まだ行っていない場合は、[送信スパム ポリシー通知の設定](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy)を検討してください。</span><span class="sxs-lookup"><span data-stu-id="77401-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="77401-105">[メッセージ トレース](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc)を使用して、イベント値 **Spam** があるかどうかを確認します。この値は送信メッセージに追加の詳細情報 (**危険度の高い配信プールを使用する**) を含みます。</span><span class="sxs-lookup"><span data-stu-id="77401-105">Use [message trace](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="77401-106">これらのメッセージについては、メッセージの内容を確認し、スパムとして考えられる可能性のあるものを確認してください。</span><span class="sxs-lookup"><span data-stu-id="77401-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="77401-107">たとえば、署名が多くのユーザーに対して問題を引き起こすことがあります。</span><span class="sxs-lookup"><span data-stu-id="77401-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="77401-108">迷惑メールとしてマークされている正当な送信メッセージの例が複数ある場合にはサポート チケットを開き、そのメッセージを誤検出としてスパム アナリストに送信するようサポート エージェントに依頼してください。</span><span class="sxs-lookup"><span data-stu-id="77401-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="77401-109">すべてのメッセージ ヘッダーを含むサンプル メッセージを提供する準備をします。</span><span class="sxs-lookup"><span data-stu-id="77401-109">Be prepared to provide sample messages that include all message headers.</span></span>
