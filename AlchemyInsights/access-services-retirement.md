---
title: Access サービスの廃止
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698687"
---
# <a name="access-services-retirement"></a>Access サービスの廃止

2017 年 3 月に MC97576 で最初に発表し、この 1 年間も引き続きご案内させていただいた通り、Access Services は廃止されます。 このプロセスの次のフェーズでは、基になるデータ ストレージとして SharePoint リストを使用する Access Web データベースを削除します。

**どのような影響がありますか?**

SharePoint Online での新しい Access データベースの作成を 2019 年 6 月以降停止し、2020 年 4 月 までにサービスと残りのすべてアプリを廃止します。

**この変更に関してどのような準備をすればよいのですか?**

組織の Access Web データベースの移行計画を作成することをお勧めします。 管理者は、[SharePoint Access アプリス キャナー](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner)を使用して、サイトが使用している Access アプリのインベントリを取得できます。

Access Web データベースのデータを移行するには、いくつかの方法があります。

- ローカル Access データベース (.ACCDB) または Excel ファイルにインポートする方法。
- Web およびモバイル デバイス用にコード不要のビジネス ソリューションを作成するための代替プラットフォームとして Microsoft PowerApps の利用可能性を検討することもお勧めします。