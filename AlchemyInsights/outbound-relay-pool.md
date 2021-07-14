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
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/08/2021
ms.locfileid: "53382029"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="1b1c0-102">送信中継プール</span><span class="sxs-lookup"><span data-stu-id="1b1c0-102">Outbound relay pool</span></span>

<span data-ttu-id="1b1c0-103">Microsoft は、Microsoft 365 経由でメールを中継または転送するための構成をいくつか変更しています。</span><span class="sxs-lookup"><span data-stu-id="1b1c0-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="1b1c0-104">特定のシナリオにおけるメッセージは、特別な中継プールを使用して Microsoft 365 経由で転送または中継されます。</span><span class="sxs-lookup"><span data-stu-id="1b1c0-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="1b1c0-105">中継プールを使用して送信したメールが、受信者の迷惑メール フォルダに入ってしまう場合があります。</span><span class="sxs-lookup"><span data-stu-id="1b1c0-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="1b1c0-106">詳細については、「[送信中継プール](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="1b1c0-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="1b1c0-107">中継プールを使用したシナリオを回避するには、転送/中継されたメッセージが以下のいずれかの条件を満たしていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="1b1c0-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="1b1c0-108">送信者は、テナントの承認済みドメインです。</span><span class="sxs-lookup"><span data-stu-id="1b1c0-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="1b1c0-109">Microsoft 365 でメッセージを受信する場合に、Sender Policy Framework (SPF) がパスします。</span><span class="sxs-lookup"><span data-stu-id="1b1c0-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="1b1c0-110">P2 送信者ドメインのドメインキー識別済みメール (DKIM) は、Microsoft 365 でメッセージを受信するときにパスします。</span><span class="sxs-lookup"><span data-stu-id="1b1c0-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="1b1c0-111">上記の条件を満たすメッセージは、中継プールを経由して中継されることはありません。</span><span class="sxs-lookup"><span data-stu-id="1b1c0-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="1b1c0-112">ドメインの MX レコードがサード パーティまたはオンプレミスのサーバーを指す場合、強化されたフィルター処理を使用して、受信メールの SPF 検証が正しいことを確認し、中継プール経由でメールを送信しないようにします。</span><span class="sxs-lookup"><span data-stu-id="1b1c0-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="1b1c0-113">**中継プールの影響を受けているかどうかは、どのように判断すればいいのでしょうか**。</span><span class="sxs-lookup"><span data-stu-id="1b1c0-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="1b1c0-114">転送されたメールや中継されたメールが上記の条件のいずれかを使用している場合、メッセージが中継プール経由で中継されることはありません。</span><span class="sxs-lookup"><span data-stu-id="1b1c0-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="1b1c0-115">ただし、メッセージが中継プール経由で送信された場合、送信サーバー IP は 40.95.0.0/16 の範囲にあり、送信サーバー名には **rly** が含まれます。</span><span class="sxs-lookup"><span data-stu-id="1b1c0-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

