---
title: ユーザーが悪意のあるメールを受信した場合
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291797"
---
# <a name="did-your-users-receive-malicious-email"></a><span data-ttu-id="b8498-102">ユーザーが悪意のあるメールを受信した場合</span><span class="sxs-lookup"><span data-stu-id="b8498-102">Did your users receive malicious email?</span></span>

- <span data-ttu-id="b8498-103">現在は、セキュリティ/コンプライアンス センターの [管理者による報告] から、悪意のあるメールを [Microsoft に報告](https://sip.protection.office.com/reportsubmission)することができます。</span><span class="sxs-lookup"><span data-stu-id="b8498-103">You can now report the malicious email to Microsoft using the [Admin Submissions in Security & Compliance Center](https://sip.protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="b8498-104">[管理者によって送信されたメッセージ](https://sip.protection.office.com/reportsubmission)がスキャンされ、次の結果が **詳細** ポップアップに表示されます。</span><span class="sxs-lookup"><span data-stu-id="b8498-104">Messages that are submitted in [admin submissions](https://sip.protection.office.com/reportsubmission) are scanned, and the following results shown in the **details** flyout:</span></span>

- <span data-ttu-id="b8498-105">配信時に送信者のメール認証に失敗した場合。</span><span class="sxs-lookup"><span data-stu-id="b8498-105">If there was a failure in the sender's email authentication at the time of delivery.</span></span>
- <span data-ttu-id="b8498-106">メッセージのセキュリティ判定に影響を与える、または上書きされる可能性があるポリシー ヒットに関する情報。</span><span class="sxs-lookup"><span data-stu-id="b8498-106">Information about any policy hits that could have affected or overridden the verdict of a message.</span></span>
- <span data-ttu-id="b8498-107">現在の爆発的な結果により、メッセージに含まれる URL またはファイルが悪意のあるものかが確認されます。</span><span class="sxs-lookup"><span data-stu-id="b8498-107">Current detonation results to see if the URLs or files contained in the message were malicious or not.</span></span>
- <span data-ttu-id="b8498-108">評価者からのフィードバック</span><span class="sxs-lookup"><span data-stu-id="b8498-108">Feedback from graders</span></span>

<span data-ttu-id="b8498-109">上書きが見つかった場合、再スキャンは数分で完了します。</span><span class="sxs-lookup"><span data-stu-id="b8498-109">If an override was found, the rescan should complete in several minutes.</span></span> <span data-ttu-id="b8498-110">メール認証に問題がなかった場合、または配信が上書きによる影響を受けなかった場合でも、評価者からのフィードバックは最大で 1 日かかる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="b8498-110">If there wasn't a problem in email authentication or if the delivery wasn't affected by an override, then the feedback from graders could take up to a day.</span></span>

<span data-ttu-id="b8498-111">メッセージ、URL またはファイル (ブロックされている場合とブロックされていない場合) の最終的な判断に同意できない場合は、再スキャンを行うために、1 日後にメッセージを再送信してください。</span><span class="sxs-lookup"><span data-stu-id="b8498-111">If you disagree with the final verdict on a message, URL or file (blocked vs. not blocked), submit the message again after a day for rescan.</span></span> <span data-ttu-id="b8498-112">メッセージを再送信した後にセキュリティ判定が変わる可能性は十分ありえます。</span><span class="sxs-lookup"><span data-stu-id="b8498-112">The chances are high that the verdict would change after submitting the message again.</span></span>

<span data-ttu-id="b8498-113">その間、[この記事](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)の手順に従って、ユーザーの受信トレイから悪意のあるメールを削除します。</span><span class="sxs-lookup"><span data-stu-id="b8498-113">Meanwhile, you can remove malicious email from user inboxes by following the instructions in [this article](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span></span>

- <span data-ttu-id="b8498-114">Microsoft Defender for Office 365 をお使いのお客様は次のサービスを利用できます。</span><span class="sxs-lookup"><span data-stu-id="b8498-114">Customers with Microsoft Defender for Office 365 can:</span></span>
    - <span data-ttu-id="b8498-115">[脅威エクスプローラーを使って不審なメールを検索して削除する](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span><span class="sxs-lookup"><span data-stu-id="b8498-115">use [Threat Explorer to Find and Delete Suspicious email](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span></span>
    - <span data-ttu-id="b8498-116">[安全なリンクを使用して悪意のある URL アクセスをブロックする](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links)</span><span class="sxs-lookup"><span data-stu-id="b8498-116">[use Safe Links to block access](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) to a malicious URL</span></span>
    - <span data-ttu-id="b8498-117">悪意のある URL をクリックしてアクセスしたユーザーを追跡する: [フィッシング URL を表示して、セキュリティ判定データをクリックします。](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span><span class="sxs-lookup"><span data-stu-id="b8498-117">track users who clicked and accessed malicious URLs: [View phishing URL and click verdict data](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span></span>
    - <span data-ttu-id="b8498-118">手動にて[自動調査を開始する](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span><span class="sxs-lookup"><span data-stu-id="b8498-118">manually [start an Automated Investigation](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span></span>

<span data-ttu-id="b8498-119">「[悪意のある URL およびファイルからの保護](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats)」の手順に従って、悪意のあるファイルおよび URL からの保護を行うこともできます。</span><span class="sxs-lookup"><span data-stu-id="b8498-119">You can also protect against malicious files and URLs by following the instructions in [Protection from malicious URLs and files](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span></span>