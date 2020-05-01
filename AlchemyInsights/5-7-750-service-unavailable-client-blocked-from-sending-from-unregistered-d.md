---
title: 1048 5.7.750 サービスは利用できません。クライアントが未登録のドメインからの送信をブロックしました
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 48b9c2de27f8d7f52215c3a3d547bdf746a3a4cd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676718"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="cc495-103">5.7.750 クライアントが未登録のドメインからの送信をブロックしました</span><span class="sxs-lookup"><span data-stu-id="cc495-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="cc495-104">(承認済みドメインおよび検証済みとして追加された) テナントでプロビジョニングされていないドメインから大量のメッセージが送信されると、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="cc495-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="cc495-105">このエラーを回避するには、証明書のドメインがプロビジョニングされたドメインである場合は、証明書ベースのメール フロー コネクタを使用できます。または、送信側のドメインをすべてプロビジョニングすることもできます。</span><span class="sxs-lookup"><span data-stu-id="cc495-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
