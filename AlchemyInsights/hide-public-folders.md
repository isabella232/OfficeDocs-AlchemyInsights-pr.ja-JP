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
# <a name="hide-public-folders"></a>パブリック フォルダーを非表示にする

**パブリック フォルダー ツリー全体を非表示にするには**:

[この](https://aka.ms/ControlPF)記事の手順を使用して、パブリック フォルダー ツリー全体を選択ユーザーまたはすべてのユーザーから非表示にします。

**特定のパブリック フォルダーを非表示にするには**:

1. パブリック フォルダーにアクセスする必要があるユーザーのアクセス許可を追加する

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. **アクセス許可** リストからユーザー **Default** を削除する:

    `Remove-PublicFolderClientPermission \test1 -User Default`
