---
title: 送信中継プール
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: d2f83b3afc4abf72a3e18bffe5ac9d6c940cc216916925338c18f0fb8a39948a
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/11/2021
ms.locfileid: "57883136"
---
# <a name="outbound-relay-pool"></a>送信中継プール

Microsoft は、Microsoft 365 経由でメールを中継または転送するための構成をいくつか変更しています。 特定のシナリオにおけるメッセージは、特別な中継プールを使用して Microsoft 365 経由で転送または中継されます。 中継プールを使用して送信したメールが、受信者の迷惑メール フォルダに入ってしまう場合があります。 詳細については、「[送信中継プール](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)」をご覧ください。

中継プールを使用したシナリオを回避するには、転送/中継されたメッセージが以下のいずれかの条件を満たしていることを確認してください。

- 送信者は、テナントの承認済みドメインです。
- Microsoft 365 でメッセージを受信する場合に、Sender Policy Framework (SPF) がパスします。
- P2 送信者ドメインのドメインキー識別済みメール (DKIM) は、Microsoft 365 でメッセージを受信するときにパスします。
 
上記の条件を満たすメッセージは、中継プールを経由して中継されることはありません。

ドメインの MX レコードがサード パーティまたはオンプレミスのサーバーを指す場合、強化されたフィルター処理を使用して、受信メールの SPF 検証が正しいことを確認し、中継プール経由でメールを送信しないようにします。

**中継プールの影響を受けているかどうかは、どのように判断すればいいのでしょうか**。

転送されたメールや中継されたメールが上記の条件のいずれかを使用している場合、メッセージが中継プール経由で中継されることはありません。 ただし、メッセージが中継プール経由で送信された場合、送信サーバー IP は 40.95.0.0/16 の範囲にあり、送信サーバー名には **rly** が含まれます。

