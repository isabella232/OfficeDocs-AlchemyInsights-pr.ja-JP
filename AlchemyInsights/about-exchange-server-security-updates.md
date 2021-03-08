---
title: Exchange Server のセキュリティ更新プログラムについて
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005482"
- "9005483"
- "9413"
- "9412"
ms.openlocfilehash: 87a5cf1ac4dfb96a5406f6b1431adb6ead074fd6
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/04/2021
ms.locfileid: "50484072"
---
# <a name="about-exchange-server-security-updates"></a>Exchange Server のセキュリティ更新プログラムについて

マイクロソフトは、オンプレミスの Exchange Server 用の一連の重要なセキュリティ更新プログラムをリリースしました。 影響を受けるサーバーのバージョンは、Exchange Server 2010、2013、2016、および 2019 の更新レベルです。 Exchange Online は影響を受けませんが、ハイブリッド構成のためにオンプレミスの Exchange サーバーがある場合、それらは潜在的に脆弱です。

オンプレミス サーバーを更新するには、少なくとも次のバージョンの Exchange を実行している必要があります。

- Exchange 2010 Service Pack 3
- Exchange Server 2013 CU 23
- Exchange Server 2016 CU 19 または CU 18
- Exchange Server 2019 CU 8 または CU 7

修正の場所については、次の発表を参照してください。[リリース: 2021 年 3 月 Exchange Server セキュリティ アップデート](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)

**重要な注意点:**

上記のリストのように、オンプレミス サーバーで必要な Exchange バージョンが実行されていない場合、更新プログラムのインストールは機能しません。

アップデートを手動でインストールする場合、重要な情報については、アップデート KB の記事の「既知の問題」セクションをお読みください。 セキュリティ更新プログラムは、昇格した CMD/PowerShell プロンプトから実行する必要があります。
