---
title: アドレス一覧でグループを表示または非表示にする手順
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 61ba34e6d554831da712a92401f26fabb02c26b7
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908349"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Microsoft 365 グループをアドレス一覧 (GAL) から非表示にする

Exchange クライアント (Outlook や OWA など) のアドレス一覧 (GAL) から Microsoft 365 グループを非表示にするには、EXO シェルで次のコマンドを使用します。

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Microsoft 365 グループを Exchange クライアントから非表示にするには、EXO シェルで次のコマンドを使用します。

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

