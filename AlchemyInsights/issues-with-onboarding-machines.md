---
title: マシンのオンボードの問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141908"
---
# <a name="issues-with-onboarding-machines"></a>マシンのオンボードの問題

MDATP サービスへのマシンのオンボードに問題がある可能性があります。 エンド ユーザーのマシンにアクセスできる場合は、次の手順を実行します。

1. [クライアント接続アナライザー](https://aka.ms/mdatpanalyzer)の診断ツールをダウンロードします。
2. 展開し、MDATPAnalyzer.cmd を実行します。
3. MDATPClientAnalyzerResult というフォルダーにある診断ログを見つけます。これは、アナライザー ツールがダウンロードされたフォルダーと同じです。
4. ログ ファイル (MDATPClientAnalyzer.txt) を確認して、接続またはインターネット プロキシ設定の問題を見つけます。