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
ms.openlocfilehash: 406bc40fbe8a6306a2f74506ef1daf70b37283d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812120"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="e07c6-102">エンドポイント DLP を構成する</span><span class="sxs-lookup"><span data-stu-id="e07c6-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="e07c6-103">Microsoft エンドポイント DLP を使用すると、 DLP の保護およびモニタリング機能を Windows 10 デバイス上の機密情報にまで拡張できます。</span><span class="sxs-lookup"><span data-stu-id="e07c6-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="e07c6-104">デバイスがデバイス管理に組み込まれたら、DLP ポリシーを作成してアイテムに保護アクションを適用できます。</span><span class="sxs-lookup"><span data-stu-id="e07c6-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="e07c6-105">アクティビティ エクスプローラーを使用して、機密アイテムのアクティビティを監視できます。</span><span class="sxs-lookup"><span data-stu-id="e07c6-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="e07c6-106">詳細については、「[デバイス管理にデバイスを組み込む](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e07c6-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="e07c6-107">エンドポイント DLP の使用を開始するには:</span><span class="sxs-lookup"><span data-stu-id="e07c6-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="e07c6-108">適切な SKU/サブスクリプションライセンスがあることを確認します。</span><span class="sxs-lookup"><span data-stu-id="e07c6-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="e07c6-109">詳細については、「[SKU/サブスクリプションライセンス](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e07c6-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="e07c6-110">デバイス管理を有効にしたり、オンボーディング ページにアクセスしたり、デバイス監視をオン/オフするために必要なアクセス許可を確認します。</span><span class="sxs-lookup"><span data-stu-id="e07c6-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="e07c6-111">詳細については、「[アクセス許可](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e07c6-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="e07c6-112">オンボーディング デバイスの手順に従って、デバイスをデバイス管理に組み込みことができます。</span><span class="sxs-lookup"><span data-stu-id="e07c6-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="e07c6-113">[M365 のコンプライアンス**設定**] に [デバイスの組み込み (プレビュー) ] オプションが表示されていない場合は、上記の適切なライセンスとアクセス許可があることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="e07c6-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="e07c6-114">詳細については、「[オンボーディング デバイス](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e07c6-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="e07c6-115">機密アイテムを保護する DLP ポリシーを作成します。</span><span class="sxs-lookup"><span data-stu-id="e07c6-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="e07c6-116">詳細については、「[エンドポイント DLP ポリシーのシナリオ](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e07c6-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="e07c6-117">Microsoft エンドポイント DLP の詳細については、「[Microsoft 365 エンドポイントのデータ損失防止について学ぶ (プレビュー)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about) 」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e07c6-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>