---
title: Microsoft 365 グループに送信されたメッセージがすべてのメンバーによって受信されません
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: d2f0674f6be135927dc5995575c14f3c2708df49
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806152"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a><span data-ttu-id="54167-102">Microsoft 365 グループに送信されたメッセージがすべてのメンバによって受信されるわけではありません</span><span class="sxs-lookup"><span data-stu-id="54167-102">Messages sent to a Microsoft 365 group are not received by all members</span></span>

<span data-ttu-id="54167-103">すべてのグループメンバーがメールを受信する購読をしていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="54167-103">Make sure that all group members have subscribed to receive the emails.</span></span> <span data-ttu-id="54167-104">詳細については、「[Outlook でグループをフォローする](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="54167-104">See [Follow a group in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span></span>  

<span data-ttu-id="54167-105">グループメールを購読しているメンバーのメッセージの状態を確認するには、次のコマンドを実行してください[EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps)。</span><span class="sxs-lookup"><span data-stu-id="54167-105">To check the message status of members who have subscribed to group emails, run the following command on [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`