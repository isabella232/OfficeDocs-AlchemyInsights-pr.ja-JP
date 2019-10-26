---
title: スパム対策-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/24/2019
ms.locfileid: "37726871"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="c622b-102">エラーコード5.7.23 のメール配信の問題を修正する</span><span class="sxs-lookup"><span data-stu-id="c622b-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="c622b-103">Web 上のパブリックに使用可能な SPF または DNS レコードチェッカーで、自分のドメインの SPF DNS レコードを確認します。</span><span class="sxs-lookup"><span data-stu-id="c622b-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="c622b-104">送信メッセージが Office 365 によってスパムとして識別され、[高リスク配信プール](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages)を経由してルーティングされていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="c622b-104">Verify that the outbound message wasn't identified as spam by Office 365 and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="c622b-105">高リスク配信プール内のメッセージは SPF チェックに合格しないため、宛先の電子メール組織からは受け付けられません。</span><span class="sxs-lookup"><span data-stu-id="c622b-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="c622b-106">問題が解決しない場合は、メールを送信しようとしているメールホストの管理者に連絡する必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="c622b-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="c622b-107">バウンスメッセージで利用できる詳細な外部エラーをメモしておいてください。</span><span class="sxs-lookup"><span data-stu-id="c622b-107">Make note of the detailed external error available in the bounce message.</span></span>  <span data-ttu-id="c622b-108">Office 365 のサポートは、さらに支援できない場合があります。</span><span class="sxs-lookup"><span data-stu-id="c622b-108">Office 365 support may not be able to assist further.</span></span>