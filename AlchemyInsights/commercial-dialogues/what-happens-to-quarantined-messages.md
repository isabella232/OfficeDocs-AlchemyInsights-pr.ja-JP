---
title: 隔離されたメッセージに起こること
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: de7ea8011af792cd01963c44f8a60915747c3c11
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751450"
---
# <a name="what-happens-to-quarantined-messages"></a><span data-ttu-id="60ec8-102">隔離されたメッセージに起こること</span><span class="sxs-lookup"><span data-stu-id="60ec8-102">What happens to quarantined messages?</span></span>

<span data-ttu-id="60ec8-103">何もしないことを選択すると、メッセージは有効期限日に Office 365 によって自動的に削除されます。</span><span class="sxs-lookup"><span data-stu-id="60ec8-103">If you choose to do nothing, the message will be deleted by Office 365 automatically upon expiration.</span></span> <span data-ttu-id="60ec8-104">次の点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="60ec8-104">Note the following:</span></span>

1. <span data-ttu-id="60ec8-105">既定で、スパム、バルク、マルウェア、およびフィッシング メッセージは、検疫に 15 日間保存されます。</span><span class="sxs-lookup"><span data-stu-id="60ec8-105">By default, spam, bulk, malware, and phishing messages are kept in quarantine for 15 days.</span></span>
2. <span data-ttu-id="60ec8-106">メール フロー ルールに一致した検疫済みメッセージは、検疫に 7 日間保存されます (この設定はカスタマイズできません)。</span><span class="sxs-lookup"><span data-stu-id="60ec8-106">A quarantined message that matches a mail flow rule is kept in quarantine for 7 days (you can't customize this).</span></span>
3. <span data-ttu-id="60ec8-107">Office 365 で検疫からメッセージが削除されると、元に戻すことはできません。</span><span class="sxs-lookup"><span data-stu-id="60ec8-107">When Office 365 deletes a message from quarantine, you can't get it back.</span></span>
4. <span data-ttu-id="60ec8-108">必要に応じて、コンテンツ フィルター ポリシーの [次の期間スパムを保持する (日)] 設定を使用して、検疫済みメッセージの保存期間を変更できます。</span><span class="sxs-lookup"><span data-stu-id="60ec8-108">If you like, you can change the retention period for quarantined messages by using the Retain spam for (days) setting in your content filter policies.</span></span>
