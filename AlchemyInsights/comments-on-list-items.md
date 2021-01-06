---
title: リスト アイテムへのコメント
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724159"
---
# <a name="comments-on-list-items"></a>リスト アイテムへのコメント

ユーザーは、リスト アイテムのすべてのコメントを表示し、アイテムに関連するコメントまたはアクティビティを表示するビューをフィルター処理できます。

ユーザーは、コメントを追加および削除する前に、次の点に注意する必要があります。

- コメントは、SharePoint 固有の権限設定に従います。
- タスク リストのように、最新のユーザー インターフェイスに表示されるようにまだ構築されていない従来のリストには、このコメント機能はありません。
- このリリースでは、Teams 内のリストにコメントすることはできません。
- コメントは検索によってインデックス化されません。

管理者は、**Set-SPOTenant** PowerShell コマンドレットの **CommentsOnListItemsDisabled** パラメータを変更して、組織レベルでこの機能を無効にすることができます。

現在、サイト レベルまたはリスト レベルでコメントを無効にすることはできません。 これらのコントロールは、おそらく 2021 年第 1 四半期に更新される予定です。
