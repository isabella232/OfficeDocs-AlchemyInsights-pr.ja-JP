---
title: ルートサイトとしてのモダン サイト
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: a0f48dc79b51168c9cc045078ad8fc7d668343c7
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327607"
---
# <a name="modern-site-as-root-site"></a>ルート サイトとしてのモダン サイト

[モダン サイトと従来のサイトのルートサイトを交換](https://docs.microsoft.com/sharepoint/modern-root-site)できるようにするために、新機能のロールアウトを開始しました。 [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) を使用して、元のサイトをアーカイブしながら、別のサイトとサイトの場所を交換します。 チーム サイト (グループに接続されていない) とコミュニケーション サイトの両方で使用することができます。

**重要**: モダン コミュニケーション サイトを作成するために、従来のルートサイトを削除しないでください。 このようなことは、Microsoft ではサポートしていません。 ルートサイトを削除すると、サイトを復元するか、同じ URL の新しいサイトが作成されるまで、組織内のすべての SharePoint サイトですべてのユーザーにアクセスできなくなります。 私たちは、メッセージ センター経由でこの機能を伝えていきます。 すぐに、ユーザーのテナントの機能が有効になります。

## <a name="known-issues-with-swapping-sites"></a>サイトの入れ替えに関する既知の問題
- ターゲット サイトでは、短時間の間、"見つかりません" (HTTP 404) というエラーを返す場合があります。
- 検索インデックスを更新するには、コンテンツが再クロールされる必要があります。 ここでは、要求される手動ステップはありません。これは自動的に行われます。
- "静的" リンクに依存するもの (ファイルの同期や OneNote ファイルなど) は、手動で修正される必要があります。
- Project Server サイトを検証し、それらが正しく関連付けられていることを確認することが必要な場合があります。 
