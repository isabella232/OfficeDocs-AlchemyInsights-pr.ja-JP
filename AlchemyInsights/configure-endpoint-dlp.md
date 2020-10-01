---
title: エンドポイント DLP を構成する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: d0363d6bdecdb266a5f4a3a14bd496ede6bb9931
ms.sourcegitcommit: 76b147af688f0dc39878a913a050c0e56af054a8
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/29/2020
ms.locfileid: "48305448"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="6eed7-102">エンドポイント DLP を構成する</span><span class="sxs-lookup"><span data-stu-id="6eed7-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="6eed7-103">Microsoft エンドポイント DLP を使用すると、 DLP の保護およびモニタリング機能を Windows 10 デバイス上の機密情報にまで拡張できます。</span><span class="sxs-lookup"><span data-stu-id="6eed7-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="6eed7-104">デバイスがデバイス管理に組み込まれたら、DLP ポリシーを作成してアイテムに保護アクションを適用できます。</span><span class="sxs-lookup"><span data-stu-id="6eed7-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="6eed7-105">アクティビティ エクスプローラーを使用して、機密アイテムのアクティビティを監視できます。</span><span class="sxs-lookup"><span data-stu-id="6eed7-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="6eed7-106">詳細については、「[デバイス管理にデバイスを組み込む](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6eed7-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="6eed7-107">エンドポイント DLP の使用を開始するには:</span><span class="sxs-lookup"><span data-stu-id="6eed7-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="6eed7-108">適切な SKU/サブスクリプションライセンスがあることを確認します。</span><span class="sxs-lookup"><span data-stu-id="6eed7-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="6eed7-109">詳細については、「[SKU/サブスクリプションライセンス](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6eed7-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="6eed7-110">デバイス管理を有効にしたり、オンボーディング ページにアクセスしたり、デバイス監視をオン/オフするために必要なアクセス許可を確認します。</span><span class="sxs-lookup"><span data-stu-id="6eed7-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="6eed7-111">詳細については、「[アクセス許可](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6eed7-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="6eed7-112">オンボーディング デバイスの手順に従って、デバイスをデバイス管理に組み込みことができます。</span><span class="sxs-lookup"><span data-stu-id="6eed7-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="6eed7-113">[M365 のコンプライアンス**設定**] に [デバイスの組み込み (プレビュー) ] オプションが表示されていない場合は、上記の適切なライセンスとアクセス許可があることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="6eed7-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="6eed7-114">詳細については、「[オンボーディング デバイス](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6eed7-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="6eed7-115">機密アイテムを保護する DLP ポリシーを作成します。</span><span class="sxs-lookup"><span data-stu-id="6eed7-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="6eed7-116">詳細については、「[エンドポイント DLP ポリシーのシナリオ](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6eed7-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="6eed7-117">Microsoft エンドポイント DLP の詳細については、「[Microsoft 365 エンドポイントのデータ損失防止について学ぶ (プレビュー)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about) 」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6eed7-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="6eed7-118">**サポートが必要な場合の重要なデータ収集手順:**</span><span class="sxs-lookup"><span data-stu-id="6eed7-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="6eed7-119">[http://aka.ms/betamdatpanalyzer](http://aka.ms/betamdatpanalyzer "http://aka.ms/betamdatpanalyzer")から MDATP クライアント アナライザ プレビューをダウンロードします</span><span class="sxs-lookup"><span data-stu-id="6eed7-119">Download MDATP Client Analyzer Preview from [http://aka.ms/betamdatpanalyzer](http://aka.ms/betamdatpanalyzer "http://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="6eed7-120">cmd ウィンドウから管理者としてツールを次のように実行します。</span><span class="sxs-lookup"><span data-stu-id="6eed7-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="6eed7-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="6eed7-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="6eed7-122">「トレースを収集する分数を入力してください:」というプロンプトが表示されたら、シナリオの実行に必要な分数を入力します</span><span class="sxs-lookup"><span data-stu-id="6eed7-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="6eed7-123">シナリオを実行する</span><span class="sxs-lookup"><span data-stu-id="6eed7-123">Run the scenario</span></span>

<span data-ttu-id="6eed7-124">サポートエージェントに提供する Zip ファイル出力を収集します。</span><span class="sxs-lookup"><span data-stu-id="6eed7-124">Collect the Zip file output to be given to the Support agent.</span></span>
