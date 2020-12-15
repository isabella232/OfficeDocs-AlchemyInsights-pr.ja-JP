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
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982625"
---
# <a name="comments-on-list-items"></a>リスト アイテムへのコメント

ユーザーはまもなくリスト アイテムへのコメントを追加したり削除したりできるようになります。 ユーザーは、リスト アイテムのすべてのコメントを表示し、アイテムに関連するコメントまたはアクティビティを表示するビューをフィルター処理できます。

**時期**:

**対象指定リリース**: 10 月中旬に段階的に展開し、11 月中旬までに完了する予定

**標準リリース**: 11 月中旬に段階的に展開し、12 月上旬までに完了する予定

**展開**: 組織全体の対象指定リリース

ユーザーは、コメントを追加および削除する前に、次の点に注意する必要があります。

- コメントは、SharePoint 固有の権限設定に従います。
- タスク リストのように、最新のユーザー インターフェイスに表示されるようにまだ構築されていない従来のリストには、このコメント機能はありません。
- このリリースでは、Teams 内のリストにコメントすることはできません。
- コメントは検索によってインデックス化されません。

管理者は、**Set-SPOTenant** PowerShell コマンドレットの **CommentsOnListItemsDisabled** パラメータを変更して、組織レベルでこの機能を無効にすることができます。

現在、サイト レベルまたはリスト レベルでコメントを無効にすることはできません。 これらのコントロールは、おそらく 2021 年第 1 四半期に更新される予定です。
