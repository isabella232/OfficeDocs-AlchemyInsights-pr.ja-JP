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
# <a name="unable-to-delete-items"></a>アイテムを削除できません

SharePoint アイテムの削除に関する問題

- アイテムを削除したり、[サイトコレクション管理者](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator)がアイテムを削除したりするための[適切な権限](https://docs.microsoft.com/sharepoint/default-sharepoint-groups)があることを必ず確認してください。

- アイテムにアイテム[保持ポリシー](https://docs.microsoft.com/office365/securitycompliance/retention-policies)が設定されていないことを確認します。

- アイテムが別のユーザーに[チェックアウト](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de)されていないことを確認します。

- 最後に、管理者は、 [SharePoint のパターンとプラクティス](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation)(PnP) を使用して、stubborn アイテムの強制削除などの複雑な管理操作を実行できます。
- [PNP ファイルの削除](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [PNP フォルダーの削除](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [PNP リストアイテムの削除](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [PNP リストを削除する](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [PNP フィールドの削除 (列)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)