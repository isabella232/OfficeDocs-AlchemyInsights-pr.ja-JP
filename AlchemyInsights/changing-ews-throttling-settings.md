---
title: EWS 調整の設定の変更
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075902"
---
# <a name="changing-ews-throttling-settings"></a>EWS 調整の設定の変更

移行中に EWS 調整ポリシーを変更できる自動テストを実行してください。 これを実行した後も、EWS のインポートはメールボックスごとに 5 分あたり 150 MB に制限されます。移行スループットを向上させるには、より多くのユーザーを同時に移行してください。

EWS 調整ポリシーの変更は、次の移行の種類 (Microsoft ツールを使用) には影響しないことに注意してください： ハイブリッド、カットオーバー/ステージド (RPC/HTTP)、IMAP、G Suite、パブリック フォルダーまたは PST インポート サービス。