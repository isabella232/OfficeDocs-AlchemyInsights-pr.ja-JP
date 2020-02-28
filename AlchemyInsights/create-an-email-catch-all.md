---
title: 電子メールのキャッチをすべて作成する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2020
ms.locfileid: "42307116"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="b88f2-102">電子メールのキャッチをすべて作成する</span><span class="sxs-lookup"><span data-stu-id="b88f2-102">Create an email catch all</span></span>

<span data-ttu-id="b88f2-103">キャッチを使用しないことをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="b88f2-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="b88f2-104">送信者にバウンスを提供することをお勧めします。メッセージが処理を実行できるように、そのメッセージをアドレス指定として配信できなかったことを知らせることができます。</span><span class="sxs-lookup"><span data-stu-id="b88f2-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="b88f2-105">また、監視対象のメールボックスを制限して、以前有効なメールアドレスのみをキャッチすることもできます。</span><span class="sxs-lookup"><span data-stu-id="b88f2-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="b88f2-106">すべてのキャッチメールボックスは、適切なスパムを受信し、ほぼ監視されていない場合は最終的にはいっぱいになることがあります。</span><span class="sxs-lookup"><span data-stu-id="b88f2-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="b88f2-107">(受信制限があります。)</span><span class="sxs-lookup"><span data-stu-id="b88f2-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="b88f2-108">続行する場合は、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="b88f2-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="b88f2-109">"すべての受信者の種類" を含む動的配布グループを作成 & ます。</span><span class="sxs-lookup"><span data-stu-id="b88f2-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="b88f2-110">メールをキャッチする専用のメールボックスを作成します。たとえば、catchall@domain.com のようにします。</span><span class="sxs-lookup"><span data-stu-id="b88f2-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="b88f2-111">特定のドメインについて、DomainType を "InternalRelay" に設定します。</span><span class="sxs-lookup"><span data-stu-id="b88f2-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="b88f2-112">後でキャッチを削除した場合は、ドメインを [権限あり] に戻してください。</span><span class="sxs-lookup"><span data-stu-id="b88f2-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="b88f2-113">メールフロートランスポートルールを次のように作成します。</span><span class="sxs-lookup"><span data-stu-id="b88f2-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="b88f2-114">送信者が組織外の場合</span><span class="sxs-lookup"><span data-stu-id="b88f2-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="b88f2-115">メッセージを Catchall@domain.com にリダイレクトします。</span><span class="sxs-lookup"><span data-stu-id="b88f2-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="b88f2-116">受信者が allusers@domain.com のメンバーである場合を除きます (配布グループにはすべてのメンバーが含まれています)。</span><span class="sxs-lookup"><span data-stu-id="b88f2-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="b88f2-117">新しいメールボックスが動的配布グループに追加されたことを確認する</span><span class="sxs-lookup"><span data-stu-id="b88f2-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
