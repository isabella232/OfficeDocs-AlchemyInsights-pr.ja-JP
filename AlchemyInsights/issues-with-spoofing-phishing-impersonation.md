---
title: スプーフィング、フィッシング、なりすましに関する問題。
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1755
ms.assetid: ''
ms.openlocfilehash: fb10c486833cfb0a1726dce69bc2176b39565e9d
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510037"
---
# <a name="issues-with-spoofing-phishing-or-impersonation"></a><span data-ttu-id="3b703-102">スプーフィング、フィッシング、なりすましに関する問題。</span><span class="sxs-lookup"><span data-stu-id="3b703-102">Issues with spoofing, phishing, or impersonation?</span></span>

<span data-ttu-id="3b703-103">Microsoft は、次の被害に遭わないようにお客様を保護します。</span><span class="sxs-lookup"><span data-stu-id="3b703-103">Learn how Microsoft protects you from:</span></span>

- <span data-ttu-id="3b703-104">「[スプーフィング](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spoofing-protection)」</span><span class="sxs-lookup"><span data-stu-id="3b703-104">[Spoofing](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spoofing-protection)</span></span>

- <span data-ttu-id="3b703-105">「[フィッシングおよびなりすまし](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-anti-phishing)」</span><span class="sxs-lookup"><span data-stu-id="3b703-105">[Phishing and impersonation](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-anti-phishing)</span></span>

<span data-ttu-id="3b703-106">追加の推奨事項:</span><span class="sxs-lookup"><span data-stu-id="3b703-106">Additional recommendations:</span></span>

- <span data-ttu-id="3b703-107">独自のドメインから送信されたように見えるスプーフィングされた送信元に対しては、[SPF](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing) と [DKIM](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email) を役立てます。</span><span class="sxs-lookup"><span data-stu-id="3b703-107">For spoofed senders that appear to come from your own domain, [SPF](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing) and [DKIM](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email) can help.</span></span>

- <span data-ttu-id="3b703-108">独自のドメインの送信者が、メール フロー ルール (トランスポート ルールとも呼ばれます) または許可リストのエントリを使用して、スパム対策フィルターを迂回できるように構成されていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="3b703-108">Verify senders in your own domain aren't configured to bypass anti-spam filtering using mail flow rules (also known as transport rules) or allow list entries.</span></span> <span data-ttu-id="3b703-109">詳細については、「[Microsoft スパム フィルターの迂回に対する注意](https://docs.microsoft.com/exchange/troubleshoot/antispam/cautions-against-bypassing-spam-filters)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3b703-109">For more information, see [Cautions against bypassing Microsoft spam filters](https://docs.microsoft.com/exchange/troubleshoot/antispam/cautions-against-bypassing-spam-filters).</span></span>

- <span data-ttu-id="3b703-110">ユーザーによって、フィッシング攻撃を許可するような[信頼できる差出人のリスト](https://support.office.com/article/BE1BAEA0-BEAB-4A30-B968-9004332336CE)のエントリが構成されていないかを確認します。</span><span class="sxs-lookup"><span data-stu-id="3b703-110">Verify that users haven't configured [Safe Senders list](https://support.office.com/article/BE1BAEA0-BEAB-4A30-B968-9004332336CE) entries that could allow phishing attacks.</span></span>

- <span data-ttu-id="3b703-111">[迷惑メール] フォルダーではなく検疫に、信頼性の高いスパムおよびフィッシング詐欺のメッセージを配信することを検討してください。</span><span class="sxs-lookup"><span data-stu-id="3b703-111">Consider delivering high-confidence spam and phishing messages to quarantine instead of the Junk Email folder.</span></span> <span data-ttu-id="3b703-112">詳細については、「[メール メッセージの検疫](https://docs.microsoft.com/microsoft-365/security/office-365-security/quarantine-email-messages)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3b703-112">For more information, see [Quarantine email messages](https://docs.microsoft.com/microsoft-365/security/office-365-security/quarantine-email-messages).</span></span>

<span data-ttu-id="3b703-113">**[Microsoft にメッセージを報告する](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2)ことは、フィルターがどのように機能しているかを知る最良の方法です。**</span><span class="sxs-lookup"><span data-stu-id="3b703-113">**[Reporting messages to Microsoft](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) is the best way to let us know how the filters are performing.**</span></span>
