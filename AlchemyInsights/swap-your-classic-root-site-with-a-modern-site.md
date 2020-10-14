---
title: モダン サイトとクラシック ルート サイトを入れ替える
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691184"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>モダン サイトとクラシック ルート サイトを入れ替える

2019 年 4 月より前に環境を設定した場合は、Microsoft PowerShell を使用して、ルート サイトをモダン サイトに変更できます。

- ルート サイトとして使用したい別のサイトをお持ちの場合は、そのサイトと[ルート サイトを置き換える (入れ替える)](https://docs.microsoft.com/sharepoint/modern-root-site) ことができます。 
    - [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) を使用して、元のサイトをアーカイブしながら、別のサイトとサイトの場所を交換します。 チーム サイト (グループに接続されていない) とコミュニケーション サイトの両方で使用することができます。 

- 間もなく、追加機能が導入されて、引き続きサイトのコンテンツを使用できるようになりますが、既存のサイトをコミュニケーション サイトに変換します。 
>[!Important]
>これらの機能は、段階的にロールアウトされます。 定期的にメッセージ センターで更新プログラムについてご確認ください。 

## <a name="known-issues-with-swapping-sites"></a>サイトの入れ替えに関する既知の問題

- ターゲット サイトでは、短時間の間、"見つかりません" (HTTP 404) というエラーを返す場合があります。
- 検索インデックスを更新するには、コンテンツが再クロールされる必要があります。 要求される手動ステップはありません。つまり、これは自動的に行われます。
- "静的" リンクに依存するもの (ファイルの同期や OneNote ファイルなど) は、手動で修正される必要があります。
- ソース サイトが組織のニュース サイトだった場合は、URL を更新します。 すべての組織のニュース サイトの一覧を取得します。
- Project Server サイトを検証し、それらが正しく関連付けられていることを確認することが必要な場合があります。
