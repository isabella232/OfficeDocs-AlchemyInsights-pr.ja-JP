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
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908349"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="776e0-102">アドレス一覧 (GAL) で Microsoft 365 グループを非表示にする</span><span class="sxs-lookup"><span data-stu-id="776e0-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="776e0-103">Microsoft 365 グループを Exchange クライアント (Outlook や OWA など) のアドレス一覧 (GAL) で非表示にするには、EXO シェルで次のコマンドを使用します。</span><span class="sxs-lookup"><span data-stu-id="776e0-103">To hide an Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="776e0-104">Microsoft 365 グループを Exchange クライアントで非表示にするには、EXO シェルで次のコマンドを使用します。</span><span class="sxs-lookup"><span data-stu-id="776e0-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

