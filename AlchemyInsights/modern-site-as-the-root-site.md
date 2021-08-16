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
ms.openlocfilehash: b42cf276a76547584c8cfd87b5a28f31d51ea7f8ca56621b22aeef01e4613ce6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000397"
---
# <a name="modern-site-as-root-site"></a>ルート サイトとしてのモダン サイト

[モダン サイトと従来のサイトのルートサイトを交換](https://docs.microsoft.com/sharepoint/modern-root-site)できるようにするために、新機能のロールアウトを開始しました。 [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) を使用して、元のサイトをアーカイブしながら、別のサイトとサイトの場所を交換します。 チーム サイト (グループに接続されていない) とコミュニケーション サイトの両方で使用することができます。

>[!Important]
> モダン コミュニケーション サイトを作成するために、従来のルート サイトを削除しないでください。 このようなことは、Microsoft ではサポートしていません。 ルートサイトを削除すると、サイトを復元するか、同じ URL の新しいサイトが作成されるまで、組織内のすべての SharePoint サイトですべてのユーザーにアクセスできなくなります。 私たちは、メッセージ センター経由でこの機能を伝えていきます。 すぐに、ユーザーのテナントの機能が有効になります。

## <a name="known-issues-with-swapping-sites"></a>サイトの入れ替えに関する既知の問題
- ターゲット サイトでは、短時間の間、"見つかりません" (HTTP 404) というエラーを返す場合があります。
- 検索インデックスを更新するには、コンテンツが再クロールされる必要があります。 ここでは、要求される手動ステップはありません。これは自動的に行われます。
- "静的" リンクに依存するもの (ファイルの同期や OneNote ファイルなど) は、手動で修正される必要があります。
- Project Server サイトを検証し、それらが正しく関連付けられていることを確認することが必要な場合があります。 
