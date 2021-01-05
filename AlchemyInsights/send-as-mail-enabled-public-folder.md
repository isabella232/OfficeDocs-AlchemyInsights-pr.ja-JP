---
title: EXO でメールが有効なパブリック フォルダーとして送信する
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ed62c6d7db0ae532f806ce4fdc48f42623bcd545
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/13/2020
ms.locfileid: "48462099"
---
# <a name="sendas-mail-enabled-public-folder"></a><span data-ttu-id="8613f-102">メールが有効なパブリック フォルダーとして送信する</span><span class="sxs-lookup"><span data-stu-id="8613f-102">SendAs Mail Enabled Public Folder</span></span>

<span data-ttu-id="8613f-103">次の例では、メールが有効なパブリック フォルダー NewPF1 の "差出人を指定して送信する" アクセス許可をユーザー Jason に割り当てています。</span><span class="sxs-lookup"><span data-stu-id="8613f-103">The following example assigns "Send As" permissions for the mail-enabled public folder NewPF1 to the user Jason.</span></span>

<span data-ttu-id="8613f-104">Add-RecipientPermission -Identity "NewPF1" -Trustee "Jason" -AccessRights "SendAs"</span><span class="sxs-lookup"><span data-stu-id="8613f-104">Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'</span></span>

<span data-ttu-id="8613f-105">詳細な構文やパラメーターの情報については、「[メールが有効なパブリック フォルダーに "差出人を指定して送信する" または "代理人として送信する" アクセス許可を割り当てる](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8613f-105">For detailed syntax and parameter information see [Assign "Send As" or "Send on Behalf" permissions for mail-enabled public folders](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span></span>

