---
title: 1048 5.7.750 サービスは利用できません。クライアントが未登録のドメインからの送信をブロックしました
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 5879c5996a28e8e9e61c696c51e7c590d1245ba1
ms.sourcegitcommit: edb9be61ff8c4df2a600f70952f6fa731c2093a9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/04/2021
ms.locfileid: "52774256"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a>5.7.750 クライアントが未登録のドメインからの送信をブロックしました

(承認済みドメインおよび検証済みとして追加された) テナントでプロビジョニングされていないドメインから大量のメッセージが送信されると、エラーが発生します。

このエラーを回避するには、証明書のドメインがプロビジョニングされたドメインである場合は、証明書ベースのメール フロー コネクタを使用できます。または、送信側のドメインをすべてプロビジョニングすることもできます。

詳細については、「[Exchange Online でエラー コード 5.7.700 から 5.7.750 までのメール配信の問題を修正する](https://go.microsoft.com/fwlink/?linkid=2164955)」を参照してください。