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
ms.openlocfilehash: d0e0285701f1a5f308bdc682abaddf5cc2d34120
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/29/2019
ms.locfileid: "37805611"
---
# <a name="hide-office-365-group-from-address-list-gal"></a><span data-ttu-id="cbb94-102">アドレス一覧 (GAL) で Office 365 グループを非表示にする</span><span class="sxs-lookup"><span data-stu-id="cbb94-102">Hide Office 365 group from address list (GAL)</span></span>

<span data-ttu-id="cbb94-103">Office 365 グループを Exchange クライアント (Outlook や OWA など) のアドレス一覧 (GAL) で非表示にするには、EXO シェルで次のコマンドを使用します。</span><span class="sxs-lookup"><span data-stu-id="cbb94-103">To hide an Office 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="cbb94-104">Office 365 グループを Exchange クライアントで非表示にするには、EXO シェルで次のコマンドを使用します。</span><span class="sxs-lookup"><span data-stu-id="cbb94-104">To hide the Office 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

