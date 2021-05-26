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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657934"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="5e641-102">エンドポイント DLP を構成する</span><span class="sxs-lookup"><span data-stu-id="5e641-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="5e641-103">Microsoft エンドポイント DLP を使用すると、 DLP の保護およびモニタリング機能を Windows 10 デバイス上の機密情報にまで拡張できます。</span><span class="sxs-lookup"><span data-stu-id="5e641-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="5e641-104">デバイスがデバイス管理に組み込まれたら、DLP ポリシーを作成してアイテムに保護アクションを適用できます。</span><span class="sxs-lookup"><span data-stu-id="5e641-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="5e641-105">アクティビティ エクスプローラーを使用して、機密アイテムのアクティビティを監視できます。</span><span class="sxs-lookup"><span data-stu-id="5e641-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="5e641-106">詳細については、「[デバイス管理にデバイスを組み込む](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5e641-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="5e641-107">エンドポイント DLP の使用を開始するには:</span><span class="sxs-lookup"><span data-stu-id="5e641-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="5e641-108">適切な SKU/サブスクリプションライセンスがあることを確認します。</span><span class="sxs-lookup"><span data-stu-id="5e641-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="5e641-109">詳細については、「[SKU/サブスクリプションライセンス](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5e641-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="5e641-p103">デバイス管理を有効にしたり、オンボーディング ページにアクセスしたり、デバイス監視をオン/オフするために必要なアクセス許可を確認します。詳細は「[アクセス許可](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5e641-p103">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring. For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="5e641-112">オンボーディング デバイスの手順に従って、デバイスをデバイス管理に組み込みことができます。</span><span class="sxs-lookup"><span data-stu-id="5e641-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="5e641-113">詳細については、「[オンボーディング デバイス](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5e641-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="5e641-114">機密アイテムを保護する DLP ポリシーを作成します。</span><span class="sxs-lookup"><span data-stu-id="5e641-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="5e641-115">詳細については、「[エンドポイント DLP ポリシーのシナリオ](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5e641-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="5e641-116">Microsoft エンドポイント DLP の詳細については、「[Microsoft 365 エンドポイントのデータ損失防止について学ぶ (プレビュー)](/microsoft-365/compliance/endpoint-dlp-learn-about) 」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5e641-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="5e641-117">**サポートが必要な場合の重要なデータ収集手順:**</span><span class="sxs-lookup"><span data-stu-id="5e641-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="5e641-118">[MDATP クライアント アナライザ プレビュー](https://aka.ms/betamdatpanalyzer)をダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="5e641-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="5e641-119">cmd ウィンドウから管理者としてツールを次のように実行します。</span><span class="sxs-lookup"><span data-stu-id="5e641-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="5e641-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="5e641-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="5e641-121">**「トレースを収集する分数を入力してください:**」というプロンプトが表示されたら、シナリオの実行に必要な分数を入力します。</span><span class="sxs-lookup"><span data-stu-id="5e641-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="5e641-122">シナリオを実行します。</span><span class="sxs-lookup"><span data-stu-id="5e641-122">Run the scenario.</span></span>

<span data-ttu-id="5e641-123">サポート エージェントに提供する Zip ファイル出力を収集します。</span><span class="sxs-lookup"><span data-stu-id="5e641-123">Collect the Zip file output to give to the Support agent.</span></span>
