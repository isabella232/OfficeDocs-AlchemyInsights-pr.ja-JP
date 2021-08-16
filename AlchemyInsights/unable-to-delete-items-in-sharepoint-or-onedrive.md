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
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038522"
---
# <a name="unable-to-delete-items"></a>アイテムが削除できない

- アイテム保持ポリシーが原因である可能性があります。この問題の原因となっているそれぞれの保留を無効にするか除外する必要があります。 アイテム保持ポリシーまたは保留を削除すると、この変更が反映されるまでに最大で 24 時間かかる場合があります。 アイテムに[アイテム保持ポリシー](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)が設定されていないことを確認します。

- サイトがストレージ上限を超えている可能性があります。[サイトのクォータ](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps)を増やし、アイテムを削除します。

- アイテムが別のユーザーに[チェックアウト](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de)されていないことを確認します。

- 最後に、管理者は [SharePoint パターンおよびプラクティス](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) を使用するようにしてください。これには、削除困難なアイテムの強制削除など、複雑な管理操作を実行できるようにする PowerShell コマンドのライブラリが含まれています。
- [PNP ファイルを削除する](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [PNP フォルダーを削除する](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [PNP リスト アイテムを削除する](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [PNP リストを削除する](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [PNP フィールド (列) を削除する](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)