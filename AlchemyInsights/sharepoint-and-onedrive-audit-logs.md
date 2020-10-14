---
title: 従来の SharePoint 監査ログ レポート
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662213"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="3dac2-102">SharePoint および OneDrive 監査ログ</span><span class="sxs-lookup"><span data-stu-id="3dac2-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="3dac2-103">SharePoint クラシック監査ログ</span><span class="sxs-lookup"><span data-stu-id="3dac2-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="3dac2-104">SPO レガシ監査を統合監査ログ (UAL) に移行しました。</span><span class="sxs-lookup"><span data-stu-id="3dac2-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="3dac2-105">すべての SPO レガシ監査レポートが UAL を介して提供され、レガシ監査信号が UAL に移行されました。</span><span class="sxs-lookup"><span data-stu-id="3dac2-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="3dac2-106">重要な変更:</span><span class="sxs-lookup"><span data-stu-id="3dac2-106">Key changes:</span></span>

* <span data-ttu-id="3dac2-107">機能としてのトリミングは使用できません。</span><span class="sxs-lookup"><span data-stu-id="3dac2-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="3dac2-108">監査する特定のイベントを選択することはできません。</span><span class="sxs-lookup"><span data-stu-id="3dac2-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="3dac2-109">既定で利用可能な監査イベントの完全なリストについては、[このドキュメント](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3dac2-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="3dac2-110">**カスタマイズされたレポート**の「**場所**」オプションは使用できません。</span><span class="sxs-lookup"><span data-stu-id="3dac2-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="3dac2-111">「**ドキュメントを開くまたはダウンロードする**」イベント オプションは利用できません。</span><span class="sxs-lookup"><span data-stu-id="3dac2-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="3dac2-112">サイト コレクションの監査設定を構成する</span><span class="sxs-lookup"><span data-stu-id="3dac2-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="3dac2-113">SharePoint と OneDrive のモダン統合監査ログをコンプライアンス センターから実行</span><span class="sxs-lookup"><span data-stu-id="3dac2-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="3dac2-114">統合監査ログを有効または無効にする</span><span class="sxs-lookup"><span data-stu-id="3dac2-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="3dac2-115">SharePoint または OneDrive で追加の構成は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="3dac2-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="3dac2-116">監査ログの検索を使用して、ファイル、フォルダー、ユーザーのアクセス許可のアクティビティを確認します。</span><span class="sxs-lookup"><span data-stu-id="3dac2-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="3dac2-117">ファイル アクティビティとページ アクティビティ</span><span class="sxs-lookup"><span data-stu-id="3dac2-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="3dac2-118">フォルダー アクティビティ</span><span class="sxs-lookup"><span data-stu-id="3dac2-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="3dac2-119">共有アクティビティとアクセス要求アクティビティ</span><span class="sxs-lookup"><span data-stu-id="3dac2-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="3dac2-120">同期アクティビティ</span><span class="sxs-lookup"><span data-stu-id="3dac2-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="3dac2-121">サイト管理アクティビティ</span><span class="sxs-lookup"><span data-stu-id="3dac2-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="3dac2-122">これらのイベントを取得する方法の詳細については、「[監査ログを検索する](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3dac2-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
