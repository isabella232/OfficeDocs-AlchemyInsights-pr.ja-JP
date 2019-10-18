---
title: 従来の SharePoint 監査ログ レポート
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068028"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="cf3cb-102">SharePoint および OneDrive 監査ログ</span><span class="sxs-lookup"><span data-stu-id="cf3cb-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="cf3cb-103">**SharePoint と OneDrive のモダン統合監査ログをコンプライアンス センターから実行**</span><span class="sxs-lookup"><span data-stu-id="cf3cb-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="cf3cb-104">統合監査ログを有効または無効にする</span><span class="sxs-lookup"><span data-stu-id="cf3cb-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="cf3cb-105">SharePoint または OneDrive で追加の構成は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="cf3cb-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="cf3cb-106">監査ログの検索を使用して、ファイル、フォルダー、ユーザーのアクセス許可のアクティビティを確認します。</span><span class="sxs-lookup"><span data-stu-id="cf3cb-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="cf3cb-107">ファイル アクティビティとページ アクティビティ</span><span class="sxs-lookup"><span data-stu-id="cf3cb-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="cf3cb-108">フォルダー アクティビティ</span><span class="sxs-lookup"><span data-stu-id="cf3cb-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="cf3cb-109">共有アクティビティとアクセス要求アクティビティ</span><span class="sxs-lookup"><span data-stu-id="cf3cb-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="cf3cb-110">同期アクティビティ</span><span class="sxs-lookup"><span data-stu-id="cf3cb-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="cf3cb-111">サイト管理アクティビティ</span><span class="sxs-lookup"><span data-stu-id="cf3cb-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="cf3cb-112">これらのイベントを取得する方法の詳細については、「[監査ログを検索する](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cf3cb-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="cf3cb-113">**SharePoint クラシック監査ログ**</span><span class="sxs-lookup"><span data-stu-id="cf3cb-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="cf3cb-114">SPO レガシー監査を統合監査ログ (UAL) に移行しました。</span><span class="sxs-lookup"><span data-stu-id="cf3cb-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="cf3cb-115">これは基本的に、すべての SPO レガシー監査レポートが UAL を介して提供され、レガシー監査信号が UAL に移行されたことを意味します。</span><span class="sxs-lookup"><span data-stu-id="cf3cb-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="cf3cb-116">重要な変更:</span><span class="sxs-lookup"><span data-stu-id="cf3cb-116">Key changes:</span></span>

- <span data-ttu-id="cf3cb-117">機能としてのトリミングは使用できません。</span><span class="sxs-lookup"><span data-stu-id="cf3cb-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="cf3cb-118">監査する特定のイベントを選択するセクションは利用できません。</span><span class="sxs-lookup"><span data-stu-id="cf3cb-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="cf3cb-119">既定で利用可能な監査イベントの完全なリストについては、[このドキュメント](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cf3cb-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="cf3cb-120">**カスタマイズされたレポート**の「場所」オプションは使用できません。</span><span class="sxs-lookup"><span data-stu-id="cf3cb-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="cf3cb-121">「ドキュメントを開くまたはダウンロードする」イベントは利用できません。</span><span class="sxs-lookup"><span data-stu-id="cf3cb-121">“Opening or downloading documents” events is NOT available.</span></span> 

