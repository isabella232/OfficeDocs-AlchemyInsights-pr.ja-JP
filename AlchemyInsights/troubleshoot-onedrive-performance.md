---
title: OneDrive のパフォーマンスのトラブルシューティング
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 4699f6113acd70b4778f9feeaeec012ff8fdd63f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757890"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="f8eaa-102">OneDrive のパフォーマンスのトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="f8eaa-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="f8eaa-103">予想よりも遅い同期が発生している場合、または OneDrive に同様のパフォーマンスの問題が発生している場合:</span><span class="sxs-lookup"><span data-stu-id="f8eaa-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="f8eaa-104">[サービスの正常性ダッシュボード](https://portal.office.com/adminportal/home?ref=/servicehealth)を使用して、既知の問題がないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="f8eaa-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="f8eaa-105">OneDrive のファイルをすべてダウンロードし、デバイス上の記憶域を使用することなく、すべてのファイルにアクセスできるようにするために、[ファイル オンデマンド機能を有効にします](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e)。</span><span class="sxs-lookup"><span data-stu-id="f8eaa-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="f8eaa-106">ネットワーク計画とパフォーマンスの[ベスト プラクティスを確認します](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance)。</span><span class="sxs-lookup"><span data-stu-id="f8eaa-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="f8eaa-107">特にデバイスを初めて同期する場合は、[アップロードとダウンロードの速度を最大化します](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43)。</span><span class="sxs-lookup"><span data-stu-id="f8eaa-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="f8eaa-108">10 万件を超えるアイテムを含むライブラリを同期している場合、OneDrive の同期が長時間停止しているように見えるか、状態に "xMB の 0KB を処理中" と表示される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f8eaa-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="f8eaa-109">[詳細については、「10 万件を超えるファイルの同期」](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa)および[「OneDrive でサポートされる 30 万ファイルの上限」](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f8eaa-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="f8eaa-p102">あるユーザーが使用制限を超えると、そのユーザー アカウントからさらに送られる要求は SharePoint Online によって短時間、調整されます。調整が有効な間、ユーザー操作はすべて調整されます。</span><span class="sxs-lookup"><span data-stu-id="f8eaa-p102">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period. All user actions are throttled while the throttle is in effect.</span></span>
