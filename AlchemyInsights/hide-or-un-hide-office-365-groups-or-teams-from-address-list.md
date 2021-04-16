---
title: Office 365 のグループまたはチームをアドレス一覧で非表示にするまたは非表示を解除する
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: 12e221c69775f3dfeed1781b70d3061e1ca0ac3b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811461"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Office 365 のグループまたはチームをアドレス一覧で非表示にするまたは非表示を解除する

Exchange クライアント (Outlook、OWA) のアドレス一覧 (GAL) で Office 365 のグループまたはチームを非表示にするまたは非表示を解除するには、次の EXO PowerShell コマンドを使用します。

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Exchange クライアント (Outlook、OWA) で Office 365 のグループまたはチームを非表示にするまたは非表示を解除するには、次の EXO PowerShell コマンドを使用します。

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- 詳しい手順については、「[Office 365 グループを GAL および Exchange クライアントで非表示にする](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)」を参照してください。
