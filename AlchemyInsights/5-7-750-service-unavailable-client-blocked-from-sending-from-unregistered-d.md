---
title: 1048 5.7.750 サービスは利用できません。クライアントが未登録のドメインからの送信をブロックしました
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 11a49add5a33073788b27fff5b2e5ec0edf7894b
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/21/2020
ms.locfileid: "43642221"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a>5.7.750 クライアントが未登録のドメインからの送信をブロックしました

このエラーは、テナントでプロビジョニングされていないドメインから大量のメッセージが送信された場合に発生します (承認済みドメインとして追加され、検証されます)。

このエラーを回避するには、証明書のドメインがプロビジョニングされたドメインである場合は、証明書ベースのメール フロー コネクタを使用できます。または、送信側のドメインをすべてプロビジョニングすることもできます。
