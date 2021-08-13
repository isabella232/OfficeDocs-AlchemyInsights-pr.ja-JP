---
title: アドレス一覧でグループを表示または非表示にする手順
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: af7085890d295cf0c41e11aaf18e404313413100cb8a1134bfac051d5fa26996
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926250"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>アドレス一覧 (GAL) で Microsoft 365 グループを非表示にする

Microsoft 365 グループを Exchange クライアント (Outlook や OWA など) のアドレス一覧 (GAL) で非表示にするには、EXO シェルで次のコマンドを使用します。

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Microsoft 365 グループを Exchange クライアントで非表示にするには、EXO シェルで次のコマンドを使用します。

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

