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
ms.openlocfilehash: 080c060f5675065704c7209bd15e4cbb1236b8db
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480688"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Microsoft 365 グループに送信されたメッセージがすべてのメンバによって受信されるわけではありません

すべてのグループメンバーがメールを受信する購読をしていることを確認してください。 詳細については、「[Outlook でグループをフォローする](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36)」を参照してください。  

グループメールを購読しているメンバーのメッセージの状態を確認するには、次のコマンドを実行してください[EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)。

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

次の EXO PowerShell コマンドを使用して、Microsoft 365 グループに送信されたメールを受信トレイで受信するようにすべてのグループ メンバーを構成します。

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

次に例を示します。

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`