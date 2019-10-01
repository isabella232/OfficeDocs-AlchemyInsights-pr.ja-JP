---
title: 迷惑メールフォルダーへの送信メール
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
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/20/2019
ms.locfileid: "37313910"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="883e6-102">迷惑メールフォルダーへの送信メール</span><span class="sxs-lookup"><span data-stu-id="883e6-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="883e6-103">送信メッセージが迷惑メールとしてマークされている場合は、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="883e6-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="883e6-104">まだ[送信スパムポリシー通知の構成](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy)を検討してください。</span><span class="sxs-lookup"><span data-stu-id="883e6-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="883e6-105">[メッセージ追跡](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc)を使用して、送信メッセージに追加の詳細情報を含むイベント値が**スパム**であるかどうかを確認します。 [**高リスク配信プールを使用**する。</span><span class="sxs-lookup"><span data-stu-id="883e6-105">Use [message trace](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="883e6-106">これらのメッセージでは、メッセージの内容をチェックして、スパムと見なされる内容を確認します。</span><span class="sxs-lookup"><span data-stu-id="883e6-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="883e6-107">たとえば、署名は多くのユーザーにとって問題を引き起こすことがあります。</span><span class="sxs-lookup"><span data-stu-id="883e6-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="883e6-108">迷惑メールとしてマークされている正当な送信メッセージの例が複数ある場合は、サポートチケットを開いて、メッセージを誤検知としてスパムアナリストに送信するようサポートエージェントに依頼します。</span><span class="sxs-lookup"><span data-stu-id="883e6-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="883e6-109">すべてのメッセージヘッダーを含むサンプルメッセージを提供できるように準備します。</span><span class="sxs-lookup"><span data-stu-id="883e6-109">Be prepared to provide sample messages that include all message headers.</span></span>
