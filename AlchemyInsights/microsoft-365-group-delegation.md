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
# <a name="microsoft-365-group-delegation"></a>Microsoft 365 グループの委任

特定のユーザーが Microsoft 365 グループとしてメッセージを送信できるように、送信者アクセス許可を割り当てることができます。  

1. Exchange Online PowerShell に接続します。  

2. 次のコマンドを実行します。  

    Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs

詳細については、「[グループとして、またはグループの代わりに送信することをメンバーに許可する](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide)」を参照してください。