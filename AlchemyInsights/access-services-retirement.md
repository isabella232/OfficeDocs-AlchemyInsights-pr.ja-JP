---
title: Access サービスの廃止
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/15/2019
ms.locfileid: "36747789"
---
# <a name="access-services-retirement"></a>Access サービスの廃止

2017 年 3 月に MC97576 で最初に発表し、この 1 年間も引き続きご案内させていただいた通り、Access Services は Office 365 で廃止されます。 このプロセスの次のフェーズでは、基になるデータ ストレージとして SharePoint リストを使用する Access Web データベースを削除します。

**どのような影響がありますか?**

SharePoint Online での新しい Access データベースの作成を 2019 年 6 月以降停止し、2020 年 4 月 までにサービスと残りのすべてアプリを廃止します。

**この変更に関してどのような準備をすればよいのですか?**

組織の Access Web データベースの移行計画を作成することをお勧めします。 管理者は、[SharePoint Access アプリス キャナー](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner)を使用して、サイトが使用している Access アプリのインベントリを取得できます。

Access Web データベースのデータを移行するには、いくつかの方法があります。

- ローカル Access データベース (.ACCDB) または Excel ファイルにインポートする方法。
- Web およびモバイル デバイス用にコード不要のビジネス ソリューションを作成するための代替プラットフォームとして Microsoft PowerApps の利用可能性を検討することもお勧めします。