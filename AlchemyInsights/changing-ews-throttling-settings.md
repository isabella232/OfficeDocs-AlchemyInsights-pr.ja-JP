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
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="89d43-102">EWS 調整の設定の変更</span><span class="sxs-lookup"><span data-stu-id="89d43-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="89d43-103">移行中に EWS 調整ポリシーを変更できる自動テストを実行してください。</span><span class="sxs-lookup"><span data-stu-id="89d43-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="89d43-104">これを実行した後も、EWS のインポートはメールボックスごとに 5 分あたり 150 MB に制限されます。移行スループットを向上させるには、より多くのユーザーを同時に移行してください。</span><span class="sxs-lookup"><span data-stu-id="89d43-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="89d43-105">EWS 調整ポリシーの変更は、次の移行の種類 (Microsoft ツールを使用) には影響しないことに注意してください： ハイブリッド、カットオーバー/ステージド (RPC/HTTP)、IMAP、G Suite、パブリック フォルダーまたは PST インポート サービス。</span><span class="sxs-lookup"><span data-stu-id="89d43-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>