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
ms.openlocfilehash: 66c76947d553c32475ebe7a11e69246b5b3a2882bb3d022873d85b93b3e87887
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945747"
---
# <a name="hide-public-folders"></a>パブリック フォルダーを非表示にする

**パブリック フォルダー ツリー全体を非表示にするには**:

[この](https://aka.ms/ControlPF)記事の手順を使用して、パブリック フォルダー ツリー全体を選択ユーザーまたはすべてのユーザーから非表示にします。

**特定のパブリック フォルダーを非表示にするには**:

1. パブリック フォルダーにアクセスする必要があるユーザーのアクセス許可を追加する

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. **アクセス許可** リストからユーザー **Default** を削除する:

    `Remove-PublicFolderClientPermission \test1 -User Default`
