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
ms.openlocfilehash: f99bb449b542760c6c8d51ee399c774fbe36e3f7f40520b5eb23f39d9d7c08dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53968382"
---
# <a name="changing-ews-throttling-settings"></a>EWS 調整の設定の変更

移行中に EWS 調整ポリシーを変更できる自動テストを実行してください。 これを実行した後も、EWS のインポートはメールボックスごとに 5 分あたり 150 MB に制限されます。移行スループットを向上させるには、より多くのユーザーを同時に移行してください。

EWS 調整ポリシーの変更は、次の移行の種類 (Microsoft ツールを使用) には影響しないことに注意してください： ハイブリッド、カットオーバー/ステージド (RPC/HTTP)、IMAP、G Suite、パブリック フォルダーまたは PST インポート サービス。