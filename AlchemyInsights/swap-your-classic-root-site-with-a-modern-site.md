---
title: 従来のルートサイトをモダンサイトと入れ替える
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
- "9000687"
- "2579"
ms.openlocfilehash: ffb1466fe436d6cab7ae5fdd60c671f5dd2654dd
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36501084"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>従来のルートサイトをモダンサイトと入れ替える

4月2019日より前に環境を設定した場合は、Microsoft PowerShell を使用してルートサイトをモダンサイトに変更することができます。

- ルートサイトとして使用する別のサイトがある場合は、ルートサイトを置き換える (スワップする) ことができます。 
    - 元のサイトをアーカイブしているときに、 [SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps)を使用してサイトの場所を別のサイトと交換します。 両方のチームサイト (グループに接続されていない) とコミュニケーションサイトで使用できます。 

- サイトのコンテンツを引き続き使用し、既存のサイトをコミュニケーションサイトに変換できる追加機能が導入されます。 
>[!Important]
>これらの機能は段階的にロールアウトされます。 引き続き Office 365 メッセージセンターで更新プログラムをチェックします。 

## <a name="known-issues-with-swapping-sites"></a>サイトのスワップに関する既知の問題

- ターゲットサイトは、短時間に "not found" (HTTP 404) エラーを返す場合があります。
- 検索インデックスを更新するには、コンテンツを再クロールする必要があります。 手動による手順は必要ありません。これは自動的に実行されます。
- "静的" リンク (ファイル同期や OneNote ファイルなど) に依存するものは、手動で修正する必要があります。
- ソースサイトが組織のニュースサイトの場合は、URL を更新します。すべての組織のニュースサイトのリストを取得します。
- Project Server サイトが正しく関連付けられていることを確認するには、そのサイトを検証する必要があります。





