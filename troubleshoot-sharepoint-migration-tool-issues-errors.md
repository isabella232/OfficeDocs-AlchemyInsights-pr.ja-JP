---
title: SharePoint 移行ツールに関する問題とエラーのトラブルシューティング
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.date: 10/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3178"
ms.assetid: ''
ms.openlocfilehash: f9f5694b1d88bccebdc5448d5629ea5120c52511
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931123"
---
# <a name="troubleshooting-sharepoint-migration-tool-issues-and-errors"></a><span data-ttu-id="ae569-102">SharePoint 移行ツールに関する問題とエラーのトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="ae569-102">Troubleshooting SharePoint Migration Tool issues and errors</span></span>

<span data-ttu-id="ae569-103">**重要**: 多くの SharePoint Online および OneDrive をご利用のお客様は、バックグラウンドで実行されるサービスに対してビジネスに不可欠なアプリケーションを実行します。</span><span class="sxs-lookup"><span data-stu-id="ae569-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="ae569-104">これには、コンテンツの移行、データ損失防止 (DLP)、およびバックアップ ソリューションが含まれます。</span><span class="sxs-lookup"><span data-stu-id="ae569-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="ae569-105">これらの前例のない時期に、リモート作業シナリオでこれまで以上にサービスに依存しているユーザーに対して、SharePoint Online および OneDrive サービスの可用性と信頼性を確保するための措置を講じています。</span><span class="sxs-lookup"><span data-stu-id="ae569-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="ae569-106">この目的をサポートするため、平日の昼間の時間帯に、バックグラウンド アプリ (移行、DLP、およびバックアップ ソリューション) の調整制限を強化しました。</span><span class="sxs-lookup"><span data-stu-id="ae569-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="ae569-107">これらのアプリのスループットは、これらの期間では非常に制限されています。</span><span class="sxs-lookup"><span data-stu-id="ae569-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="ae569-108">ただし、同地域の夕方および週末には、サービスはバックグラウンド アプリからの非常に大量のリクエストを処理する準備が整います。</span><span class="sxs-lookup"><span data-stu-id="ae569-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="ae569-109">**一般的な問題とエラー**</span><span class="sxs-lookup"><span data-stu-id="ae569-109">**Common issues and errors**</span></span>

<span data-ttu-id="ae569-110">SharePoint 移行ツール (SPMT) を使用するときに、一般的な問題やエラーが発生する場合があります。</span><span class="sxs-lookup"><span data-stu-id="ae569-110">You may encounter some common issues and errors when using the SharePoint Migration Tool (SPMT).</span></span> <span data-ttu-id="ae569-111">詳細については、次のリンクを参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae569-111">Please reference the links below for more information.</span></span>

* [<span data-ttu-id="ae569-112">SharePoint 移行ツールの一般的な問題とエラーのトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="ae569-112">Troubleshooting common SPMT issues and errors</span></span>](https://docs.microsoft.com/sharepointmigration/troubleshooting-common-spmt-issues)
* [<span data-ttu-id="ae569-113">SharePoint 移行ツールのインストールに関する問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="ae569-113">Troubleshooting SPMT install issues</span></span>](https://docs.microsoft.com/sharepointmigration/spmt-install-issues)