---
title: Exchange Online でパブリック フォルダーの予定表を作成して共有する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "634"
- "3500007"
ms.openlocfilehash: d8b28d373db21da42b90aeef75139affd802a5d2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47804411"
---
# <a name="create-and-share-public-folder-calendars-in-exchange-online"></a><span data-ttu-id="dfc46-102">Exchange Online でパブリック フォルダーの予定表を作成して共有する</span><span class="sxs-lookup"><span data-stu-id="dfc46-102">Create and share public folder calendars in Exchange Online</span></span>

<span data-ttu-id="dfc46-103">Outlook デスクトップ クライアントからのみ、パブリック フォルダーに予定表を作成できます。</span><span class="sxs-lookup"><span data-stu-id="dfc46-103">You can create a calendar in the Public folder only from the Outlook desktop client.</span></span> <span data-ttu-id="dfc46-104">次の手順を使用して、パブリック フォルダーの予定表をセットアップします。</span><span class="sxs-lookup"><span data-stu-id="dfc46-104">Use these steps to set up public folder calendars:</span></span>

1. <span data-ttu-id="dfc46-105">パブリック フォルダーが Exchange Online に展開されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="dfc46-105">Ensure public folders are deployed in Exchange Online.</span></span> <span data-ttu-id="dfc46-106">詳細については、「[パブリック フォルダーのメールボックスを作成する](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/create-public-folder-mailbox)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="dfc46-106">For more info, see [Create a public folder mailbox](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/create-public-folder-mailbox).</span></span> 

2. <span data-ttu-id="dfc46-107">パブリック フォルダーを作成するために必要なアクセス許可が割り当てられていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="dfc46-107">Ensure you're assigned necessary access permissions to create the public folder.</span></span> <span data-ttu-id="dfc46-108">詳細については、「[Exchange Server のパブリック フォルダーへのアクセス許可](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="dfc46-108">For more info, see [Public folder permissions for Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span></span> 
  
3. <span data-ttu-id="dfc46-109">Outlook デスクトップ クライアントにログインし、パブリック フォルダーの展開にアクセスできることを確認します。</span><span class="sxs-lookup"><span data-stu-id="dfc46-109">Log in to the Outlook desktop client and ensure you can access your public folder deployment.</span></span>

    <span data-ttu-id="dfc46-110">Outlook デスクトップ クライアントを使用してパブリック フォルダーにアクセスできない場合は、「[Exchange Online ユーザーが Outlook または OWA を使用してパブリック フォルダーに接続できない](https://aka.ms/pfcte)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="dfc46-110">If you're having trouble accessing public folders by using the Outlook desktop client, see [Exchange Online users can't connect to public folders by using Outlook or OWA](https://aka.ms/pfcte).</span></span>

4. <span data-ttu-id="dfc46-111">新しいパブリック フォルダーの予定表の種類を作成します。</span><span class="sxs-lookup"><span data-stu-id="dfc46-111">Create a new public folder calendar type.</span></span>

<span data-ttu-id="dfc46-112">パブリック フォルダーは、既定で他のすべてのユーザーと共有されます。</span><span class="sxs-lookup"><span data-stu-id="dfc46-112">The public folder is shared to all other users by default.</span></span> <span data-ttu-id="dfc46-113">パブリック フォルダーの所有者は、Outlook デスクトップ クライアントからアクセス許可を変更できます。</span><span class="sxs-lookup"><span data-stu-id="dfc46-113">Owner of the public folder can change the permissions from Outlook desktop client.</span></span> <span data-ttu-id="dfc46-114">詳細については、「[Exchange Server のパブリック フォルダーへのアクセス許可](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="dfc46-114">For more info, see [Public folder permissions for Exchange Server](https://support.microsoft.com/help/2573274/public-folder-permissions-for-exchange-server).</span></span>

<span data-ttu-id="dfc46-115">**注** パブリック フォルダーの予定表は組織内で使用するように設計されており、インターネット上で公開することはできません。</span><span class="sxs-lookup"><span data-stu-id="dfc46-115">**Note** Public folder calendars are designed to be used within the organization and can't be published on the Internet.</span></span> <span data-ttu-id="dfc46-116">インターネットで予定表を公開する場合は、共有メールボックスを使用します。</span><span class="sxs-lookup"><span data-stu-id="dfc46-116">Use a shared mailbox if your intention is to publish a calendar on the  Internet.</span></span>