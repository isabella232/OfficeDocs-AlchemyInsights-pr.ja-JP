---
title: ルートサイトとしてのモダンサイト
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: d5ea73c967013822854dbd408d4628d991c90378
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620764"
---
# <a name="modern-site-as-root-site"></a>ルートサイトとしてのモダンサイト

従来のサイトのルートサイトをモダンサイトと入れ替えることができる新機能のロールアウトを開始しました。 元のサイトをアーカイブしているときに、 [SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps)を使用してサイトの場所を別のサイトと交換します。 両方のチームサイト (グループに接続されていない) とコミュニケーションサイトで使用できます。 

>[!Important]
> モダンコミュニケーションサイトを作成するために、従来のルートサイトを削除しないでください。 これは Microsoft ではサポートされていません。 ルートサイトを削除すると、サイトを復元するか、同じ URL で新しいサイトを作成するまで、組織内のすべての SharePoint サイトがすべてのユーザーに対してアクセスできなくなります。 この機能は、メッセージセンター経由で通信します。 この機能は、すぐにテナントでオンになるはずです。

## <a name="known-issues-with-swapping-sites"></a>サイトのスワップに関する既知の問題
- ターゲットサイトは、短時間に "not found" (HTTP 404) エラーを返す場合があります。
- 検索インデックスを更新するには、コンテンツを再クロールする必要があります。 ここでは手動での手順は必要ありませんが、これは自動的に実行されます。
- "静的" リンク (ファイル同期や OneNote ファイルなど) に依存するものは、手動で修正する必要があります。
- Project Server サイトが正しく関連付けられていることを確認するには、そのサイトを検証する必要があります。 
