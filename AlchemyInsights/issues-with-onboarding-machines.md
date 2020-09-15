---
title: マシンのオンボードの問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: c3203ed68eb19d5f6d75eb2269094bb0422b14cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47676887"
---
# <a name="issues-with-onboarding-machines"></a>マシンのオンボードの問題

MDATP サービスへのマシンのオンボードに問題がある可能性があります。 エンド ユーザーのマシンにアクセスできる場合は、次の手順を実行します。

1. [クライアント接続アナライザー](https://aka.ms/mdatpanalyzer)の診断ツールをダウンロードします。
2. 展開し、MDATPAnalyzer.cmd を実行します。
3. MDATPClientAnalyzerResult というフォルダーにある診断ログを見つけます。これは、アナライザー ツールがダウンロードされたフォルダーと同じです。
4. ログ ファイル (MDATPClientAnalyzer.txt) を確認して、接続またはインターネット プロキシ設定の問題を見つけます。