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
ms.openlocfilehash: b25e6d144dcefcfed4258e78ad5cfd4089ba7d1e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558658"
---
# <a name="unable-to-delete-items"></a>アイテムが削除できない

SharePoint アイテムの削除に問題がある場合

- アイテムを削除するための[適切なアクセス許可](https://docs.microsoft.com/sharepoint/default-sharepoint-groups)があること、または[サイト コレクション管理者](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator)がアイテムを削除しようとしていることを必ず確認します。

- アイテムに[保持ポリシー](https://docs.microsoft.com/office365/securitycompliance/retention-policies)が設定されていないことを確認します。

- アイテムが別のユーザーに[チェックアウト](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de)されていないことを確認します。

- 最後に、管理者は [SharePoint パターンおよびプラクティス](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) を使用するようにしてください。これには、削除困難なアイテムの強制削除など、複雑な管理操作を実行できるようにする PowerShell コマンドのライブラリが含まれています。
- [PNP ファイルを削除する](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [PNP フォルダーを削除する](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [PNP リスト アイテムを削除する](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [PNP リストを削除する](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [PNP フィールド (列) を削除する](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)