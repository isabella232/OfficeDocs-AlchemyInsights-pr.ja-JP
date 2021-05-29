---
title: Edge ブラウザーを使用するとインジケーターが機能しない
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676609"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="b8a69-102">Edge ブラウザーを使用するとインジケーターが機能しない</span><span class="sxs-lookup"><span data-stu-id="b8a69-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="b8a69-103">インジケーターを作成した後、Edge (スマートスクリーン) によって受け入れられません。</span><span class="sxs-lookup"><span data-stu-id="b8a69-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="b8a69-104">詳細については、「[IP および URL/ドメインのインジケーターを作成する](/microsoft-365/security/defender-endpoint/indicator-ip-domain)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b8a69-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="b8a69-105">手順 1: 次のことを確認する</span><span class="sxs-lookup"><span data-stu-id="b8a69-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="b8a69-106">インジケーターが正しいことを確認します (IP/URL にタイプミスがないこと、正しいアクション、正しい RBAC グループ)。</span><span class="sxs-lookup"><span data-stu-id="b8a69-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="b8a69-107">潜在的な待機時間を考慮し、インジケーターを作成してから最低 2 時間待ちます。</span><span class="sxs-lookup"><span data-stu-id="b8a69-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="b8a69-108">システムが Microsoft Defender for Endpoint にオンボードされていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="b8a69-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="b8a69-109">システムがクラウドと通信できることを確認します。</span><span class="sxs-lookup"><span data-stu-id="b8a69-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="b8a69-110">[テスト サイト](https://demo.smartscreen.msft.net)に移動し、スマートスクリーンが有効になっていて到達可能であることを確認します。</span><span class="sxs-lookup"><span data-stu-id="b8a69-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="b8a69-111">手順 2: 潜在的な問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="b8a69-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="b8a69-112">クライアントが要件を満たしていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="b8a69-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="b8a69-113">詳細については、「[IP および URL/ドメインのインジケーターを作成する](/microsoft-365/security/defender-endpoint/indicator-ip-domain)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b8a69-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="b8a69-114">Edge ブラウザーの最新バージョンを実行していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="b8a69-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="b8a69-115">最新バージョンを確認するには、「[お使いの Microsoft Edge のバージョンを確認する](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b8a69-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="b8a69-116">Edge ブラウザーを再起動します。</span><span class="sxs-lookup"><span data-stu-id="b8a69-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="b8a69-117">インジケーターをセットアップしたサイトに移動します。</span><span class="sxs-lookup"><span data-stu-id="b8a69-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="b8a69-118">サイトが期待どおりに表示されない場合は、手順 3 に進みます。</span><span class="sxs-lookup"><span data-stu-id="b8a69-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="b8a69-119">手順 3: データを収集する</span><span class="sxs-lookup"><span data-stu-id="b8a69-119">Step 3: Collect data</span></span>

- <span data-ttu-id="b8a69-120">**MDEClientAnalyzer** 診断データを収集します。</span><span class="sxs-lookup"><span data-stu-id="b8a69-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="b8a69-121">手順については、「[Microsoft Defender for Endpoints へのマシンのオンボードに関する問題](issues-with-onboarding-machines.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b8a69-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="b8a69-122">Fiddler トレースのインストールと収集に慣れている場合は、「[Telerik Fiddler](http://www.telerik.com/fiddler)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b8a69-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="b8a69-123">Microsoft サポートからのガイダンスを希望する場合は、下の [サポート] アイコンを選択してサポート ケースを開きます。</span><span class="sxs-lookup"><span data-stu-id="b8a69-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
