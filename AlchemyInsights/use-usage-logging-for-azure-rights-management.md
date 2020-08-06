---
title: Azure Rights Management の利用状況ログを使用する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5506"
- "9002281"
ms.openlocfilehash: 606fcdc5394edab26c60925af28cf2d938aac172
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2020
ms.locfileid: "46556254"
---
# <a name="use-usage-logging-for-azure-rights-management"></a><span data-ttu-id="6cc8e-102">Azure Rights Management の利用状況ログを使用する</span><span class="sxs-lookup"><span data-stu-id="6cc8e-102">Use usage logging for Azure Rights Management</span></span>

<span data-ttu-id="6cc8e-103">既定では、すべてのお客様に対して保護の利用状況ログが有効になっています。</span><span class="sxs-lookup"><span data-stu-id="6cc8e-103">By default, protection usage logging is enabled for all customers.</span></span> <span data-ttu-id="6cc8e-104">ログは、テナントの Azure ストレージに一連の BLOB として書き込まれます。</span><span class="sxs-lookup"><span data-stu-id="6cc8e-104">Logs are written as a series of blobs in Azure storage for your tenant.</span></span> <span data-ttu-id="6cc8e-105">保護アクションの実行後、ほとんどのログが表示されるまで、最大 15 分かかります。</span><span class="sxs-lookup"><span data-stu-id="6cc8e-105">After a protection action, it might take up to 15 minutes for most logs to appear.</span></span>

<span data-ttu-id="6cc8e-106">保護の利用状況ログを使用して次のことができます。</span><span class="sxs-lookup"><span data-stu-id="6cc8e-106">You can use protection usage logs to:</span></span>

- <span data-ttu-id="6cc8e-107">ビジネスの分析情報の確認</span><span class="sxs-lookup"><span data-stu-id="6cc8e-107">Analyze business insights</span></span>

- <span data-ttu-id="6cc8e-108">不正使用の監視</span><span class="sxs-lookup"><span data-stu-id="6cc8e-108">Monitor for abuse</span></span>

- <span data-ttu-id="6cc8e-109">フォレンジック解析の実行</span><span class="sxs-lookup"><span data-stu-id="6cc8e-109">Perform forensic analysis</span></span>

<span data-ttu-id="6cc8e-110">詳細については、「[Azure Information Protection の保護利用状況のログおよび分析](https://docs.microsoft.com/azure/information-protection/log-analyze-usage)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6cc8e-110">For more information, see [Logging and analyzing the protection usage from Azure Information Protection](https://docs.microsoft.com/azure/information-protection/log-analyze-usage).</span></span>

<span data-ttu-id="6cc8e-111">クライアントの利用状況ログの詳細については、「[管理者ガイド: Azure Information Protection クライアント ファイルおよびクライアントの利用状況ログ](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-files-and-logging)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6cc8e-111">For information about client usage logging, see [Admin Guide: Azure Information Protection client files and client usage logging](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-files-and-logging).</span></span>

<span data-ttu-id="6cc8e-112">その他の情報については、次を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6cc8e-112">For additional information, see:</span></span>

- <span data-ttu-id="6cc8e-113">[Azure Information Protection の要件](https://docs.microsoft.com/azure/information-protection/get-started/requirements)。</span><span class="sxs-lookup"><span data-stu-id="6cc8e-113">[Azure Information Protection requirements](https://docs.microsoft.com/azure/information-protection/get-started/requirements).</span></span>
    
- <span data-ttu-id="6cc8e-114">[チュートリアル: Azure Information Protection ポリシー設定を構成し、新しいラベルを作成する](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)。</span><span class="sxs-lookup"><span data-stu-id="6cc8e-114">[Tutorial: Configure Azure Information Protection policy settings and create a new label](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial).</span></span>