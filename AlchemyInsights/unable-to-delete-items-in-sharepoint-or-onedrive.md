---
title: SharePoint または OneDrive のアイテムを削除できません
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
ms.openlocfilehash: b25e6d144dcefcfed4258e78ad5cfd4089ba7d1e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558658"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="bf34d-102">アイテムを削除できません</span><span class="sxs-lookup"><span data-stu-id="bf34d-102">Unable to delete items</span></span>

<span data-ttu-id="bf34d-103">SharePoint アイテムの削除に関する問題</span><span class="sxs-lookup"><span data-stu-id="bf34d-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="bf34d-104">アイテムを削除したり、[サイトコレクション管理者](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator)がアイテムを削除したりするための[適切な権限](https://docs.microsoft.com/sharepoint/default-sharepoint-groups)があることを必ず確認してください。</span><span class="sxs-lookup"><span data-stu-id="bf34d-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="bf34d-105">アイテムにアイテム[保持ポリシー](https://docs.microsoft.com/office365/securitycompliance/retention-policies)が設定されていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="bf34d-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="bf34d-106">アイテムが別のユーザーに[チェックアウト](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de)されていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="bf34d-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="bf34d-107">最後に、管理者は、 [SharePoint のパターンとプラクティス](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation)(PnP) を使用して、stubborn アイテムの強制削除などの複雑な管理操作を実行できます。</span><span class="sxs-lookup"><span data-stu-id="bf34d-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="bf34d-108">PNP ファイルの削除</span><span class="sxs-lookup"><span data-stu-id="bf34d-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="bf34d-109">PNP フォルダーの削除</span><span class="sxs-lookup"><span data-stu-id="bf34d-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="bf34d-110">PNP リストアイテムの削除</span><span class="sxs-lookup"><span data-stu-id="bf34d-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="bf34d-111">PNP リストを削除する</span><span class="sxs-lookup"><span data-stu-id="bf34d-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="bf34d-112">PNP フィールドの削除 (列)</span><span class="sxs-lookup"><span data-stu-id="bf34d-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)