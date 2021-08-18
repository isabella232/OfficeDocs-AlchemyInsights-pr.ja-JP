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
ms.openlocfilehash: 204b2c1777f76f11663b2735b784cbb56f1f1aba891628fb46ef37b501c9ff85
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086133"
---
# <a name="send-as-microsoft-365-group"></a>Microsoft 365 グループとして送信

特定のユーザーが Microsoft 365 グループとしてメッセージを送信できるように、送信者アクセス許可を割り当てることができます。  

1. Exchange Online PowerShell に接続します。  

2. 次のコマンドを実行します。  

    Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs

詳細については、「[グループとして、またはグループの代わりに送信することをメンバーに許可する](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide)」を参照してください。