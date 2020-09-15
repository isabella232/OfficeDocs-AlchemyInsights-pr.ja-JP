---
title: Catch All メールを作成する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712991"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="d160d-102">Catch All メールを作成する</span><span class="sxs-lookup"><span data-stu-id="d160d-102">Create an email catch all</span></span>

<span data-ttu-id="d160d-103">Catch All の使用は避けることを強く推奨します。</span><span class="sxs-lookup"><span data-stu-id="d160d-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="d160d-104">送信者が処置をとることができるように、送信者に返信し、送信者のメッセージが送信先に配信されなかったことを通知することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="d160d-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="d160d-105">以前の有効なメール アドレスのみをキャッチするように監視するメールボックスを限定することもできます。</span><span class="sxs-lookup"><span data-stu-id="d160d-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="d160d-106">Catch All メールボックスは大量の迷惑メールを受信するため、厳重に監視されていない場合、最終的にはいっぱいになってしまいます。</span><span class="sxs-lookup"><span data-stu-id="d160d-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="d160d-107">(受信数には制限があります。)</span><span class="sxs-lookup"><span data-stu-id="d160d-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="d160d-108">続行する場合は、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="d160d-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="d160d-109">"すべての種類の受信者を含める" という動的配布グループを作成する。</span><span class="sxs-lookup"><span data-stu-id="d160d-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="d160d-110">catchall@domain.com などのメールをキャッチする専用のメールボックスを作成する。</span><span class="sxs-lookup"><span data-stu-id="d160d-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="d160d-111">特定のドメインについては、DomainType を "InternalRelay" に設定します。</span><span class="sxs-lookup"><span data-stu-id="d160d-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="d160d-112">後で Catch All を削除する場合は、必ずドメインを [権限あり] に戻してください。</span><span class="sxs-lookup"><span data-stu-id="d160d-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="d160d-113">メールフローのトランスポート ルールの作成方法は次のとおりです:</span><span class="sxs-lookup"><span data-stu-id="d160d-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="d160d-114">送信者が "組織外" のユーザーの場合</span><span class="sxs-lookup"><span data-stu-id="d160d-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="d160d-115">メッセージを Catchall@domain.com にリダイレクトする</span><span class="sxs-lookup"><span data-stu-id="d160d-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="d160d-116">ただし受信者が allusers@domain.com のメンバーである場合を除く (配布グループはすべてのメンバーを含む)</span><span class="sxs-lookup"><span data-stu-id="d160d-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="d160d-117">新しいメールボックスが動的配布グループに追加されたことを確認する</span><span class="sxs-lookup"><span data-stu-id="d160d-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
