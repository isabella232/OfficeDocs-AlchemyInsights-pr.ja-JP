---
title: 'チームのサインインエラーの対処: AADSTS9000411'
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
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821992"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="7973c-102">チームのサインインエラーの対処: AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="7973c-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="7973c-103">Microsoft Teams にサインインすると、次のエラーが表示されることがあります。 **"申し訳ございませんが、AADSTS9000411 でのサインインで問題が発生しています。要求の形式が正しくありません。パラメーター 「login_hint」 が重複しています。"**</span><span class="sxs-lookup"><span data-stu-id="7973c-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="7973c-104">この問題に対処するには、Microsoft Teams クライアントが更新されていることをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="7973c-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="7973c-105">クライアントの更新の詳細については、 「[Microsoft Teams の更新プログラム](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7973c-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="7973c-106">何らかの理由でクライアントを更新できない場合、クライアントをログオフすると、キャッシュされているほとんどのデータがクリアされます。</span><span class="sxs-lookup"><span data-stu-id="7973c-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="7973c-107">ただし、ログオフ/ログオン後も問題が解決しない場合は、Teams を終了し、次の操作を行って、クライアント キャッシュをクリアします。</span><span class="sxs-lookup"><span data-stu-id="7973c-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="7973c-108">Microsoft Teams を終了します。</span><span class="sxs-lookup"><span data-stu-id="7973c-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="7973c-109">%appdata%\microsoft\teams に移動し、すべてのファイルを削除します。</span><span class="sxs-lookup"><span data-stu-id="7973c-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="7973c-110">Microsoft Teams をもう一度開きます。</span><span class="sxs-lookup"><span data-stu-id="7973c-110">Reopen Microsoft Teams.</span></span>
