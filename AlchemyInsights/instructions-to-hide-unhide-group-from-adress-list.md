---
title: アドレス一覧でグループを表示または非表示にする手順
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 1ad9ab294d46ca0fc88a454e3503ddcf80398896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663014"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>アドレス一覧 (GAL) で Microsoft 365 グループを非表示にする

Microsoft 365 グループを Exchange クライアント (Outlook や OWA など) のアドレス一覧 (GAL) で非表示にするには、EXO シェルで次のコマンドを使用します。

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Microsoft 365 グループを Exchange クライアントで非表示にするには、EXO シェルで次のコマンドを使用します。

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

