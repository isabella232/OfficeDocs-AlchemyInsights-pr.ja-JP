---
title: 1048 5.7.750 サービスは利用できません。クライアントが未登録のドメインからの送信をブロックしました
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom: 1048
ms.openlocfilehash: 5eb42679f123fcd1b680327329721cb47e18e11a
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/22/2019
ms.locfileid: "31030756"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="7d01b-103">5.7.750 クライアントが未登録のドメインからの送信をブロックしました</span><span class="sxs-lookup"><span data-stu-id="7d01b-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="7d01b-104">(承認済みドメインおよび検証済みとして追加された) Office 365 でプロビジョニングされていないドメインから大量のメッセージが送信されると、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="7d01b-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in Office 365 (added as accepted domains and validated).</span></span>
  
<span data-ttu-id="7d01b-105">このエラーを回避するには、証明書のドメインがプロビジョニングされたドメインである場合は、証明書ベースのメール フロー コネクタを使用できます。または、送信側のドメインをすべてプロビジョニングすることもできます。</span><span class="sxs-lookup"><span data-stu-id="7d01b-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
  

