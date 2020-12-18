---
title: SharePoint または OneDrive でアイテムを削除できない
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: db45aa8df40484fdcda7c430f1ca27482a1dd4ce
ms.sourcegitcommit: a9415f3ae8c7ba267b5134bcbdc1e070cea41a0f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/12/2020
ms.locfileid: "49019588"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="3289c-102">アイテムが削除できない</span><span class="sxs-lookup"><span data-stu-id="3289c-102">Unable to delete items</span></span>

- <span data-ttu-id="3289c-103">アイテム保持ポリシーが原因である可能性があります。この問題の原因となっているそれぞれの保留を無効にするか除外する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3289c-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="3289c-104">アイテム保持ポリシーまたは保留を削除すると、この変更が反映されるまでに最大で 24 時間かかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="3289c-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="3289c-105">アイテムに[アイテム保持ポリシー](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)が設定されていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="3289c-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="3289c-106">サイトがストレージ上限を超えている可能性があります。[サイトのクォータ](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps)を増やし、アイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="3289c-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

- <span data-ttu-id="3289c-107">アイテムが別のユーザーに[チェックアウト](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de)されていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="3289c-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="3289c-108">最後に、管理者は [SharePoint パターンおよびプラクティス](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) を使用するようにしてください。これには、削除困難なアイテムの強制削除など、複雑な管理操作を実行できるようにする PowerShell コマンドのライブラリが含まれています。</span><span class="sxs-lookup"><span data-stu-id="3289c-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="3289c-109">PNP ファイルを削除する</span><span class="sxs-lookup"><span data-stu-id="3289c-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="3289c-110">PNP フォルダーを削除する</span><span class="sxs-lookup"><span data-stu-id="3289c-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="3289c-111">PNP リスト アイテムを削除する</span><span class="sxs-lookup"><span data-stu-id="3289c-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="3289c-112">PNP リストを削除する</span><span class="sxs-lookup"><span data-stu-id="3289c-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="3289c-113">PNP フィールド (列) を削除する</span><span class="sxs-lookup"><span data-stu-id="3289c-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)