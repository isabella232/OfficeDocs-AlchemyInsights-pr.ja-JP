---
title: 1049 スパム対策 4.5.3 受信者が多すぎます (AS780090)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1049"
- "3100024"
ms.assetid: fa3d4be9-c90a-4926-9754-4b708b038bf6
ms.openlocfilehash: 841691026560692942dfd78442e91f2b57fcbb63
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35357034"
---
# <a name="453-too-many-recipients-as780090"></a><span data-ttu-id="af8f1-102">4.5.3 受信者が多すぎます (AS780090)</span><span class="sxs-lookup"><span data-stu-id="af8f1-102">4.5.3 Too many recipients (AS780090)</span></span>

<span data-ttu-id="af8f1-103">このエラーは、ソース IP アドレスからのメール トラフィック量が、ソース IP アドレスの評価に基づいて制限を超える場合 (または評価が不十分な場合) に発生します。</span><span class="sxs-lookup"><span data-stu-id="af8f1-103">This error occurs when the volume of email traffic from the source IP address exceeds the limit based on the reputation (or lack of reputation) of source IP address.</span></span>

<span data-ttu-id="af8f1-p101">ソース IP アドレスからのメールのブロックは、1 時間以内に期限が切れます。ソース IP アドレスがお客様のオンプレミスのメール サーバーの場合、メール フロー コネクタの構成を確認してください。この動作が 1 時間以上継続する場合は、サポートに連絡してソース IP アドレスの例外を申請してください。</span><span class="sxs-lookup"><span data-stu-id="af8f1-p101">Blocking email from the source IP address will expire within an hour. If the source IP address is an on-premises email server that belongs to you, verify the configuration of the mail flow connector. If the behavior continues for more than an hour, contact support to request an exception for the source IP address.</span></span>
