---
title: EWS 調整の設定の変更
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818041"
---
# <a name="changing-ews-throttling-settings"></a>EWS 調整の設定の変更

移行中に EWS 調整ポリシーを変更できる自動テストを実行してください。 これを実行した後も、EWS のインポートはメールボックスごとに 5 分あたり 150 MB に制限されます。移行スループットを向上させるには、より多くのユーザーを同時に移行してください。

EWS 調整ポリシーの変更は、次の移行の種類 (Microsoft ツールを使用) には影響しないことに注意してください： ハイブリッド、カットオーバー/ステージド (RPC/HTTP)、IMAP、G Suite、パブリック フォルダーまたは PST インポート サービス。