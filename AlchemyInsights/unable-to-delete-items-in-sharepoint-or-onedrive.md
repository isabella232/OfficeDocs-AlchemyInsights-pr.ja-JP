---
title: SharePoint または OneDrive でアイテムを削除できない
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: cc19fcb6603160032dac52b1ec9e194a90b7891f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049522"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="113c3-102">アイテムが削除できない</span><span class="sxs-lookup"><span data-stu-id="113c3-102">Unable to delete items</span></span>

<span data-ttu-id="113c3-103">SharePoint アイテムの削除に問題がある場合</span><span class="sxs-lookup"><span data-stu-id="113c3-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="113c3-104">アイテムを削除するための[適切なアクセス許可](https://docs.microsoft.com/sharepoint/default-sharepoint-groups)があること、または[サイト コレクション管理者](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator)がアイテムを削除しようとしていることを必ず確認します。</span><span class="sxs-lookup"><span data-stu-id="113c3-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="113c3-105">アイテムに[保持ポリシー](https://docs.microsoft.com/office365/securitycompliance/retention-policies)が設定されていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="113c3-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="113c3-106">アイテムが別のユーザーに[チェックアウト](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de)されていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="113c3-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="113c3-107">最後に、管理者は [SharePoint パターンおよびプラクティス](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) を使用するようにしてください。これには、削除困難なアイテムの強制削除など、複雑な管理操作を実行できるようにする PowerShell コマンドのライブラリが含まれています。</span><span class="sxs-lookup"><span data-stu-id="113c3-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="113c3-108">PNP ファイルを削除する</span><span class="sxs-lookup"><span data-stu-id="113c3-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="113c3-109">PNP フォルダーを削除する</span><span class="sxs-lookup"><span data-stu-id="113c3-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="113c3-110">PNP リスト アイテムを削除する</span><span class="sxs-lookup"><span data-stu-id="113c3-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="113c3-111">PNP リストを削除する</span><span class="sxs-lookup"><span data-stu-id="113c3-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="113c3-112">PNP フィールド (列) を削除する</span><span class="sxs-lookup"><span data-stu-id="113c3-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)