---
title: パブリック フォルダーのアクセス許可の変更
ms.author: dmaguire
author: msdmaguire
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "633"
- "3500007"
ms.assetid: 0c37ab75-c81c-44e7-bda8-ea43263f9fdf
ms.openlocfilehash: a2a902e8fdfd8628772364c173979c633d25a169
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47714252"
---
# <a name="changing-public-folder-permissions"></a><span data-ttu-id="e946c-102">パブリック フォルダーのアクセス許可の変更</span><span class="sxs-lookup"><span data-stu-id="e946c-102">Changing public folder permissions</span></span>

<span data-ttu-id="e946c-p101">パブリック フォルダーのアクセス許可は、Outlook のユーザーと管理者が変更できます。管理者は、次の手順を実行して Exchange 管理センター (EAC) からアクセス許可を制御することもできます。</span><span class="sxs-lookup"><span data-stu-id="e946c-p101">Public folder permissions can be changed by users and administrators in Outlook. Administrators can also control permissions from the Exchange Admin Center (EAC), by doing the following:</span></span>
  
1. <span data-ttu-id="e946c-105">Microsoft 365 管理センターで、[**管理センター**] \> [**Exchange**] の順に移動します。</span><span class="sxs-lookup"><span data-stu-id="e946c-105">In the Microsoft 365 admin center, go to **Admin centers** \> **Exchange**.</span></span>

2. <span data-ttu-id="e946c-106">**パブリック フォルダー**を選択します。</span><span class="sxs-lookup"><span data-stu-id="e946c-106">Select **Public folders**.</span></span>

3. <span data-ttu-id="e946c-p102">そこから、セキュリティ グループをアクセス許可に割り当てることで、個々のパブリック フォルダーに対するアクセス許可を変更できます。エンド ユーザーがパブリック フォルダーのアクセス許可を変更するには、そのユーザーがそのフォルダーの所有者権限を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e946c-p102">From there, you can change permissions for individual public folders by assigning security groups to permissions. For an end user to change public folder permissions, the user needs to have Owner rights on the folder.</span></span>

<span data-ttu-id="e946c-109">パブリック フォルダーのアクセス許可の問題のトラブルシューティングを行うには、「[パブリック フォルダーのアクセス許可の問題を診断および修正する方法](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues)」に記載されている手順に従ってください。</span><span class="sxs-lookup"><span data-stu-id="e946c-109">Please follow the procedure described in [How to diagnose and fix public folder permission issues](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) to troubleshoot public folder permission issues.</span></span>

<span data-ttu-id="e946c-110">**メモ**: パブリック フォルダーのアクセス許可を変更しようとする際に発生する可能性がある既知の問題がいくつかあります。</span><span class="sxs-lookup"><span data-stu-id="e946c-110">**Note**: There are several known issues you might encounter when you try to change permissions on public folders.</span></span> <span data-ttu-id="e946c-111">詳細については、次の記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e946c-111">See the following articles for more information.</span></span>

- [<span data-ttu-id="e946c-112">EAC でパブリック フォルダーのサブフォルダーにアクセス許可を適用できない</span><span class="sxs-lookup"><span data-stu-id="e946c-112">Can't apply permissions to public folder subfolders in EAC</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/can%E2%80%99t-apply-permissions-public-folder-subfolders)

- [<span data-ttu-id="e946c-113">パブリック フォルダーへアクセスすると "メールボックスがローカル フォレストで見つかりません" というエラーが表示される</span><span class="sxs-lookup"><span data-stu-id="e946c-113">"The mailbox is not found in the local forest" error when you access public folders</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/mailbox-not-found-local-forest-public-folder)
