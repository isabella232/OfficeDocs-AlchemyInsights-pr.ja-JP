---
title: Access services の廃止
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 5f171050479f34077f3dc155bec40437f86b84c0
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35359356"
---
# <a name="access-services-retirement"></a>Access services の廃止

MC97576 で最初に発表されたように、2017年3月、年3月に、過去1年間のアクセスサービスは Office 365 から廃止されました。 このプロセスの次のフェーズでは、基になるデータストレージとして SharePoint リストを使用する Access Web データベースを削除します。

**どのような影響がありますか?**

2019年6月以降、SharePoint Online の新しい Access データベースの作成を停止し、サービスおよび残りのアプリを4月2020にシャットダウンします。

**この変更を準備するために必要な作業**

組織の Access web データベースの移行計画を作成することをお勧めします。 管理者は、 [SharePoint access アプリスキャナー](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner)を使用して、サイトが使用している access アプリのインベントリを取得できます。

Access web データベースのデータを移行するには、いくつかの方法があります。

- ローカル Access データベース (にインポートします。ACCDB) または Excel ファイルにします。
- また、web およびモバイルデバイス用のコードなしのビジネスソリューションを作成するための代替プラットフォームとして Microsoft PowerApps を使用することをお勧めします。