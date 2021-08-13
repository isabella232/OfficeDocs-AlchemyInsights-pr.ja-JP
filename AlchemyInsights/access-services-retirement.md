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
ms.openlocfilehash: 32da879de230dc0ed99563ad881ab5b2479b8453933a127961a26d619e108ab9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938700"
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