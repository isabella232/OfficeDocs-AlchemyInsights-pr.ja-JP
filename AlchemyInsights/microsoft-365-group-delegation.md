---
title: Microsoft 365 グループの委任
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: f6a72a96c4fb984ec24b5da75f668ecb3a4b0dbb
ms.sourcegitcommit: 28ee2811e69b6355b5ba7daf4a156c046d7ffc33
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/19/2020
ms.locfileid: "46815250"
---
# <a name="microsoft-365-group-delegation"></a><span data-ttu-id="6e7b6-102">Microsoft 365 グループの委任</span><span class="sxs-lookup"><span data-stu-id="6e7b6-102">Microsoft 365 group delegation</span></span>

<span data-ttu-id="6e7b6-103">特定のユーザーが Microsoft 365 グループとしてメッセージを送信できるように、送信者アクセス許可を割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="6e7b6-103">You can assign Send As permissions to allow specific users to send messages as a Microsoft 365 group:</span></span>  

1. <span data-ttu-id="6e7b6-104">Exchange Online PowerShell に接続します。</span><span class="sxs-lookup"><span data-stu-id="6e7b6-104">Connect to Exchange Online PowerShell.</span></span>  

2. <span data-ttu-id="6e7b6-105">次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="6e7b6-105">Run the following command:</span></span>  

    <span data-ttu-id="6e7b6-106">Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs</span><span class="sxs-lookup"><span data-stu-id="6e7b6-106">Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs</span></span>

<span data-ttu-id="6e7b6-107">詳細については、「[グループとして、またはグループの代わりに送信することをメンバーに許可する](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6e7b6-107">For more information, see [Allow members to send as or send on behalf of a group](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span></span>