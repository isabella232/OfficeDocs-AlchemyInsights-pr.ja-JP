---
title: SharePoint または OneDrive でアイテムを削除できない
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: d25214f26a3168e3e350b5cc31ca870e65d48ad9
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35366538"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="96df9-102">アイテムが削除できない</span><span class="sxs-lookup"><span data-stu-id="96df9-102">Unable to delete items</span></span>

<span data-ttu-id="96df9-103">アイテムの削除に問題がある場合</span><span class="sxs-lookup"><span data-stu-id="96df9-103">Having issues deleting items?</span></span>

- <span data-ttu-id="96df9-104">アイテムを削除するための[適切なアクセス許可](https://docs.microsoft.com/sharepoint/default-sharepoint-groups)があること、または[サイト コレクション管理者](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator)がアイテムを削除しようとしていることを必ず確認します。</span><span class="sxs-lookup"><span data-stu-id="96df9-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="96df9-105">アイテムに[保持ポリシー](https://docs.microsoft.com/office365/securitycompliance/retention-policies)が設定されていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="96df9-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="96df9-106">アイテムが別のユーザーに[チェックアウト](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de)されていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="96df9-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="96df9-107">最後に、管理者は [SharePoint パターンおよびプラクティス](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) を使用するようにしてください。これには、削除困難なアイテムの強制削除など、複雑な管理操作を実行できるようにする PowerShell コマンドのライブラリが含まれています。</span><span class="sxs-lookup"><span data-stu-id="96df9-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="96df9-108">PNP ファイルを削除する</span><span class="sxs-lookup"><span data-stu-id="96df9-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="96df9-109">PNP フォルダーを削除する</span><span class="sxs-lookup"><span data-stu-id="96df9-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="96df9-110">PNP リスト アイテムを削除する</span><span class="sxs-lookup"><span data-stu-id="96df9-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="96df9-111">PNP リストを削除する</span><span class="sxs-lookup"><span data-stu-id="96df9-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="96df9-112">PNP フィールド (列) を削除する</span><span class="sxs-lookup"><span data-stu-id="96df9-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)