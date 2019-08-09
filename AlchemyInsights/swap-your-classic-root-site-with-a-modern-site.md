---
title: モダン サイトとクラシック ルート サイトを入れ替える
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "2579"
- "9000687"
ms.openlocfilehash: dad7d7a52222dc09aea532714a93ca89c0d9ae19
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/07/2019
ms.locfileid: "36249510"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>モダン サイトとクラシック ルート サイトを入れ替える

2019 年 4 月より前に環境を設定した場合は、Microsoft PowerShell を使用して、ルート サイトをモダン サイトに変更できます。

- ルート サイトとして使用したい別のサイトをお持ちの場合は、そのサイトとルート サイトを置き換える (入れ替える) ことができます。 
    - [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) を使用して、元のサイトをアーカイブしながら、別のサイトとサイトの場所を交換します。 チーム サイト (グループに接続されていない) とコミュニケーション サイトの両方で使用できます。 

- 間もなく、追加機能が導入されて、引き続きサイトのコンテンツを使用できるようになりますが、既存のサイトをコミュニケーション サイトに変換します。 
>[!Important]
>これらの機能は、段階的にロールアウトされます。 更新プログラムに関しては、引き続き Office 365 メッセージ センターでご確認ください。 

## <a name="known-issues-with-swapping-sites"></a>サイトの入れ替えに関する既知の問題

- ターゲット サイトでは、短時間の間、"見つかりません" (HTTP 404) というエラーを返す場合があります。
- 検索インデックスを更新するには、コンテンツが再クロールされる必要があります。 要求される手動ステップはありません。つまり、これは自動的に行われます。
- "静的" リンクに依存するもの (ファイルの同期や OneNote ファイルなど) は、手動で修正される必要があります。
- ソース サイトが組織のニュース サイトだった場合は、URL を更新します。 すべての組織のニュース サイトの一覧を取得します。
- Project Server サイトを検証し、それらが正しく関連付けられていることを確認することが必要な場合があります。





