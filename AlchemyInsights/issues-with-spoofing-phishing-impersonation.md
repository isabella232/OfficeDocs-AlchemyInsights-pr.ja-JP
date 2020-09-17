---
title: スプーフィング、フィッシング、なりすましに関する問題。
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1755
ms.assetid: ''
ms.openlocfilehash: 92e7f611b08a5457e52be248982785b2dc2ddabc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773024"
---
# <a name="issues-with-spoofing-phishing-or-impersonation"></a><span data-ttu-id="9cddd-102">スプーフィング、フィッシング、なりすましに関する問題。</span><span class="sxs-lookup"><span data-stu-id="9cddd-102">Issues with spoofing, phishing, or impersonation?</span></span>

<span data-ttu-id="9cddd-103">Microsoft は、次の被害に遭わないようにお客様を保護します。</span><span class="sxs-lookup"><span data-stu-id="9cddd-103">Learn how Microsoft protects you from:</span></span>

- <span data-ttu-id="9cddd-104">「[スプーフィング](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spoofing-protection)」</span><span class="sxs-lookup"><span data-stu-id="9cddd-104">[Spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spoofing-protection)</span></span>

- <span data-ttu-id="9cddd-105">「[フィッシングおよびなりすまし](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-anti-phishing)」</span><span class="sxs-lookup"><span data-stu-id="9cddd-105">[Phishing and impersonation](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-anti-phishing)</span></span>

<span data-ttu-id="9cddd-106">追加の推奨事項:</span><span class="sxs-lookup"><span data-stu-id="9cddd-106">Additional recommendations:</span></span>

- <span data-ttu-id="9cddd-107">独自のドメインから送信されたように見えるスプーフィングされた送信元に対しては、[SPF](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing) と [DKIM](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email) を役立てます。</span><span class="sxs-lookup"><span data-stu-id="9cddd-107">For spoofed senders that appear to come from your own domain, [SPF](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing) and [DKIM](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email) can help.</span></span>

- <span data-ttu-id="9cddd-108">独自のドメインの送信者が、メール フロー ルール (トランスポート ルールとも呼ばれます) または許可リストのエントリを使用して、スパム対策フィルターを迂回できるように構成されていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="9cddd-108">Verify senders in your own domain aren't configured to bypass anti-spam filtering using mail flow rules (also known as transport rules) or allow list entries.</span></span> <span data-ttu-id="9cddd-109">詳細については、「[Microsoft スパム フィルターの迂回に対する注意](https://docs.microsoft.com/exchange/troubleshoot/antispam/cautions-against-bypassing-spam-filters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9cddd-109">For more information, see [Cautions against bypassing Microsoft spam filters](https://docs.microsoft.com/exchange/troubleshoot/antispam/cautions-against-bypassing-spam-filters).</span></span>

- <span data-ttu-id="9cddd-110">ユーザーによって、フィッシング攻撃を許可するような[信頼できる差出人のリスト](https://support.office.com/article/BE1BAEA0-BEAB-4A30-B968-9004332336CE)のエントリが構成されていないかを確認します。</span><span class="sxs-lookup"><span data-stu-id="9cddd-110">Verify that users haven't configured [Safe Senders list](https://support.office.com/article/BE1BAEA0-BEAB-4A30-B968-9004332336CE) entries that could allow phishing attacks.</span></span>

- <span data-ttu-id="9cddd-111">[迷惑メール] フォルダーではなく検疫に、信頼性の高いスパムおよびフィッシング詐欺のメッセージを配信することを検討してください。</span><span class="sxs-lookup"><span data-stu-id="9cddd-111">Consider delivering high-confidence spam and phishing messages to quarantine instead of the Junk Email folder.</span></span> <span data-ttu-id="9cddd-112">詳細については、「[メール メッセージの検疫](https://docs.microsoft.com/microsoft-365/security/office-365-security/quarantine-email-messages)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9cddd-112">For more information, see [Quarantine email messages](https://docs.microsoft.com/microsoft-365/security/office-365-security/quarantine-email-messages).</span></span>

<span data-ttu-id="9cddd-113">**[Microsoft にメッセージを報告する](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2)ことは、フィルターがどのように機能しているかを知る最良の方法です。**</span><span class="sxs-lookup"><span data-stu-id="9cddd-113">**[Reporting messages to Microsoft](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) is the best way to let us know how the filters are performing.**</span></span>
