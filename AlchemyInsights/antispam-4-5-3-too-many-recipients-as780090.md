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
ms.custom: 1049
ms.assetid: fa3d4be9-c90a-4926-9754-4b708b038bf6
ms.openlocfilehash: f6dd8e544a6d2715f1eb8f5c62ad23a162f879fa
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "34755676"
---
# <a name="453-too-many-recipients-as780090"></a><span data-ttu-id="4ab10-102">4.5.3 受信者が多すぎます (AS780090)</span><span class="sxs-lookup"><span data-stu-id="4ab10-102">4.5.3 Too many recipients (AS780090)</span></span>

<span data-ttu-id="4ab10-103">このエラーは、ソース IP アドレスからのメール トラフィック量が、ソース IP アドレスの評価に基づいて制限を超える場合 (または評価が不十分な場合) に発生します。</span><span class="sxs-lookup"><span data-stu-id="4ab10-103">This error occurs when the volume of email traffic from the source IP address exceeds the limit based on the reputation (or lack of reputation) of source IP address.</span></span>

<span data-ttu-id="4ab10-p101">ソース IP アドレスからのメールのブロックは、1 時間以内に期限が切れます。ソース IP アドレスがお客様のオンプレミスのメール サーバーの場合、メール フロー コネクタの構成を確認してください。この動作が 1 時間以上継続する場合は、サポートに連絡してソース IP アドレスの例外を申請してください。</span><span class="sxs-lookup"><span data-stu-id="4ab10-p101">Blocking email from the source IP address will expire within an hour. If the source IP address is an on-premises email server that belongs to you, verify the configuration of the mail flow connector. If the behavior continues for more than an hour, contact support to request an exception for the source IP address.</span></span>
