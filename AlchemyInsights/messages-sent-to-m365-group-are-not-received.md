---
title: Microsoft 365 グループに送信されたメッセージがすべてのメンバーによって受信されません
ms.author: pebaum
author: pebaum
manager: mnirkhe
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 39a4f8115a4742947b3e6394396be5ce3b01e772
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430688"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Microsoft 365 グループに送信されたメッセージがすべてのメンバによって受信されるわけではありません

すべてのグループメンバーがメールを受信する購読をしていることを確認してください。 詳細については、「[Outlook でグループをフォローする](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36)」を参照してください。  

グループメールを購読しているメンバーのメッセージの状態を確認するには、次のコマンドを実行してください[EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)。

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

次の EXO PowerShell コマンドを使用して、Microsoft 365 グループに送信されたメールを受信トレイで受信するようにすべてのグループ メンバーを構成します。

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`