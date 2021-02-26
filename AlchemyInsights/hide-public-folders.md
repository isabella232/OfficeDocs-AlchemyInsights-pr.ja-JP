---
title: パブリック フォルダーを非表示にする
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315567"
---
# <a name="hide-public-folders"></a><span data-ttu-id="6091f-102">パブリック フォルダーを非表示にする</span><span class="sxs-lookup"><span data-stu-id="6091f-102">Hide public folders</span></span>

<span data-ttu-id="6091f-103">**パブリック フォルダー ツリー全体を非表示にするには**:</span><span class="sxs-lookup"><span data-stu-id="6091f-103">**To hide entire public folder tree**:</span></span>

<span data-ttu-id="6091f-104">[この](https://aka.ms/ControlPF)記事の手順を使用して、パブリック フォルダー ツリー全体を選択ユーザーまたはすべてのユーザーから非表示にします。</span><span class="sxs-lookup"><span data-stu-id="6091f-104">Use the steps in [this](https://aka.ms/ControlPF) article to hide entire public folder tree from selective or all users.</span></span>

<span data-ttu-id="6091f-105">**特定のパブリック フォルダーを非表示にするには**:</span><span class="sxs-lookup"><span data-stu-id="6091f-105">**To hide a specific public folder**:</span></span>

1. <span data-ttu-id="6091f-106">パブリック フォルダーにアクセスする必要があるユーザーのアクセス許可を追加する</span><span class="sxs-lookup"><span data-stu-id="6091f-106">Add permissions for users who need to access the public folder</span></span>

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. <span data-ttu-id="6091f-107">**アクセス許可** リストからユーザー **Default** を削除する:</span><span class="sxs-lookup"><span data-stu-id="6091f-107">Remove the user **Default** from the **permission** list:</span></span>

    `Remove-PublicFolderClientPermission \test1 -User Default`
