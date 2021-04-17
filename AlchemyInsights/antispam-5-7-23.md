---
title: スパム対策 - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821416"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="c0662-102">エラー コード 5.7.23 に関するメール配信の問題を修正する</span><span class="sxs-lookup"><span data-stu-id="c0662-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="c0662-103">Web 上で一般公開されている SPF または DNS レコード チェックで、自分のドメインの SPF DNS レコードを確認します。</span><span class="sxs-lookup"><span data-stu-id="c0662-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="c0662-104">Microsoft により送信メッセージがスパムとして特定されて、[高リスク配信プール](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)経由でルーティングされなかったことを確認します。</span><span class="sxs-lookup"><span data-stu-id="c0662-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="c0662-105">高リスク配信プールのメッセージは SPF チェックに合格しないため、送信先のメール組織によって承認されません。</span><span class="sxs-lookup"><span data-stu-id="c0662-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="c0662-106">問題が解決しない場合は、メール送信先のメール ホスト管理者への連絡が必要な場合があります。</span><span class="sxs-lookup"><span data-stu-id="c0662-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="c0662-107">バウンス メッセージに表示される詳細な外部エラーをメモします。</span><span class="sxs-lookup"><span data-stu-id="c0662-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="c0662-108">Microsoft のサポートでは、これ以上のアシスタントは提供できない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="c0662-108">Microsoft support may not be able to assist further.</span></span>
