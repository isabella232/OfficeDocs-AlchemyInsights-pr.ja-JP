---
title: ユーザーが悪意のあるメールを受信した場合
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 425f9ba488fd69b8c5ea29636bccccd995bf48fd
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51815251"
---
# <a name="did-your-users-receive-malicious-email"></a><span data-ttu-id="5bb4c-102">ユーザーが悪意のあるメールを受信した場合</span><span class="sxs-lookup"><span data-stu-id="5bb4c-102">Did your users receive malicious email?</span></span>

- <span data-ttu-id="5bb4c-103">現在は、セキュリティ/コンプライアンス センターの [管理者による報告] から、悪意のあるメールを [Microsoft に報告](https://sip.protection.office.com/reportsubmission)することができます。</span><span class="sxs-lookup"><span data-stu-id="5bb4c-103">You can now report the malicious email to Microsoft using the [Admin Submissions in Security & Compliance Center](https://sip.protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="5bb4c-104">[管理者によって送信されたメッセージ](https://sip.protection.office.com/reportsubmission)がスキャンされ、次の結果が **詳細** ポップアップに表示されます。</span><span class="sxs-lookup"><span data-stu-id="5bb4c-104">Messages that are submitted in [admin submissions](https://sip.protection.office.com/reportsubmission) are scanned, and the following results shown in the **details** flyout:</span></span>

- <span data-ttu-id="5bb4c-105">配信時に送信者のメール認証に失敗した場合。</span><span class="sxs-lookup"><span data-stu-id="5bb4c-105">If there was a failure in the sender's email authentication at the time of delivery.</span></span>
- <span data-ttu-id="5bb4c-106">メッセージのセキュリティ判定に影響を与える、または上書きされる可能性があるポリシー ヒットに関する情報。</span><span class="sxs-lookup"><span data-stu-id="5bb4c-106">Information about any policy hits that could have affected or overridden the verdict of a message.</span></span>
- <span data-ttu-id="5bb4c-107">現在の爆発的な結果により、メッセージに含まれる URL またはファイルが悪意のあるものかが確認されます。</span><span class="sxs-lookup"><span data-stu-id="5bb4c-107">Current detonation results to see if the URLs or files contained in the message were malicious or not.</span></span>
- <span data-ttu-id="5bb4c-108">評価者からのフィードバック</span><span class="sxs-lookup"><span data-stu-id="5bb4c-108">Feedback from graders</span></span>

<span data-ttu-id="5bb4c-109">上書きが見つかった場合、再スキャンは数分で完了します。</span><span class="sxs-lookup"><span data-stu-id="5bb4c-109">If an override was found, the rescan should complete in several minutes.</span></span> <span data-ttu-id="5bb4c-110">メール認証に問題がなかった場合、または配信が上書きによる影響を受けなかった場合でも、評価者からのフィードバックは最大で 1 日かかる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="5bb4c-110">If there wasn't a problem in email authentication or if the delivery wasn't affected by an override, then the feedback from graders could take up to a day.</span></span>

<span data-ttu-id="5bb4c-111">メッセージ、URL またはファイル (ブロックされている場合とブロックされていない場合) の最終的な判断に同意できない場合は、再スキャンを行うために、1 日後にメッセージを再送信してください。</span><span class="sxs-lookup"><span data-stu-id="5bb4c-111">If you disagree with the final verdict on a message, URL or file (blocked vs. not blocked), submit the message again after a day for rescan.</span></span> <span data-ttu-id="5bb4c-112">メッセージを再送信した後にセキュリティ判定が変わる可能性は十分ありえます。</span><span class="sxs-lookup"><span data-stu-id="5bb4c-112">The chances are high that the verdict would change after submitting the message again.</span></span>

<span data-ttu-id="5bb4c-113">その間、[この記事](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)の手順に従って、ユーザーの受信トレイから悪意のあるメールを削除します。</span><span class="sxs-lookup"><span data-stu-id="5bb4c-113">Meanwhile, you can remove malicious email from user inboxes by following the instructions in [this article](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span></span>

- <span data-ttu-id="5bb4c-114">Microsoft Defender for Office 365 をお使いのお客様は次のサービスを利用できます。</span><span class="sxs-lookup"><span data-stu-id="5bb4c-114">Customers with Microsoft Defender for Office 365 can:</span></span>
    - <span data-ttu-id="5bb4c-115">[脅威エクスプローラーを使って不審なメールを検索して削除する](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span><span class="sxs-lookup"><span data-stu-id="5bb4c-115">use [Threat Explorer to Find and Delete Suspicious email](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span></span>
    - <span data-ttu-id="5bb4c-116">[安全なリンクを使用して悪意のある URL アクセスをブロックする](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links)</span><span class="sxs-lookup"><span data-stu-id="5bb4c-116">[use Safe Links to block access](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) to a malicious URL</span></span>
    - <span data-ttu-id="5bb4c-117">悪意のある URL をクリックしてアクセスしたユーザーを追跡する: [フィッシング URL を表示して、セキュリティ判定データをクリックします。](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span><span class="sxs-lookup"><span data-stu-id="5bb4c-117">track users who clicked and accessed malicious URLs: [View phishing URL and click verdict data](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span></span>
    - <span data-ttu-id="5bb4c-118">手動にて[自動調査を開始する](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span><span class="sxs-lookup"><span data-stu-id="5bb4c-118">manually [start an Automated Investigation](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span></span>

<span data-ttu-id="5bb4c-119">「[悪意のある URL およびファイルからの保護](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats)」の手順に従って、悪意のあるファイルおよび URL からの保護を行うこともできます。</span><span class="sxs-lookup"><span data-stu-id="5bb4c-119">You can also protect against malicious files and URLs by following the instructions in [Protection from malicious URLs and files](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span></span>