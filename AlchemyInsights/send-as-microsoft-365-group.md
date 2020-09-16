---
title: Microsoft 365 グループとして送信
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 51bd8a10c3da23941cc16d7ba860406f8477044a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740156"
---
# <a name="send-as-microsoft-365-group"></a><span data-ttu-id="35ef7-102">Microsoft 365 グループとして送信</span><span class="sxs-lookup"><span data-stu-id="35ef7-102">Send As Microsoft 365 group</span></span>

<span data-ttu-id="35ef7-103">特定のユーザーが Microsoft 365 グループとしてメッセージを送信できるように、送信者アクセス許可を割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="35ef7-103">You can assign Send As permissions to allow specific users to send messages as a Microsoft 365 group:</span></span>  

1. <span data-ttu-id="35ef7-104">Exchange Online PowerShell に接続します。</span><span class="sxs-lookup"><span data-stu-id="35ef7-104">Connect to Exchange Online PowerShell.</span></span>  

2. <span data-ttu-id="35ef7-105">次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="35ef7-105">Run the following command:</span></span>  

    <span data-ttu-id="35ef7-106">Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs</span><span class="sxs-lookup"><span data-stu-id="35ef7-106">Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs</span></span>

<span data-ttu-id="35ef7-107">詳細については、「[グループとして、またはグループの代わりに送信することをメンバーに許可する](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="35ef7-107">For more information, see [Allow members to send as or send on behalf of a group](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span></span>