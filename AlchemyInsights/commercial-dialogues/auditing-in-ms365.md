---
title: Microsoft 365 での監査
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: c07981bfae40d74deb1a2f143ce51da69b51a69f
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2021
ms.locfileid: "50484120"
---
# <a name="auditing-in-microsoft-365"></a><span data-ttu-id="8d5a4-102">Microsoft 365 での監査</span><span class="sxs-lookup"><span data-stu-id="8d5a4-102">Auditing in Microsoft 365</span></span>

<span data-ttu-id="8d5a4-103">Microsoft 365 での監査について知っておくべきことがいくつかあります。</span><span class="sxs-lookup"><span data-stu-id="8d5a4-103">Here are a few things you should know about auditing in Microsoft 365:</span></span>

1. <span data-ttu-id="8d5a4-104">Exchange 管理者のアクティビティは、既定で監査されます。</span><span class="sxs-lookup"><span data-stu-id="8d5a4-104">Exchange admin activities are audited by default.</span></span>
1. <span data-ttu-id="8d5a4-105">現在、すべてのユーザーに対してメールボックス監査を既定でオンにしています。</span><span class="sxs-lookup"><span data-stu-id="8d5a4-105">We're in the process of turning on mailbox auditing by default for all users.</span></span> <span data-ttu-id="8d5a4-106">詳細については、[こちら](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171)をクリックしてください。</span><span class="sxs-lookup"><span data-stu-id="8d5a4-106">To read more about this, click [here](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171).</span></span> <span data-ttu-id="8d5a4-107">それまでは、1 人または組織全体で手動で有効にする手順が必要な場合は、下の [メールボックスの監査を有効にする] ボタンを選択してください。</span><span class="sxs-lookup"><span data-stu-id="8d5a4-107">Until then, if you want instructions to manually enable it for one person or an entire organization, choose the Turn on mailbox auditing button below.</span></span>
1. <span data-ttu-id="8d5a4-108">Microsoft 365 グループ メールボックスとパブリック フォルダー メールボックスは、監査ログをサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="8d5a4-108">Microsoft 365 Groups mailboxes and Public Folder mailboxes do not support audit logging.</span></span>
1. <span data-ttu-id="8d5a4-109">SharePoint および OneDrive の場合、監査を有効にするために追加の構成は必要ありません。</span><span class="sxs-lookup"><span data-stu-id="8d5a4-109">For SharePoint/OneDrive, there is no additional configuration required to enabled auditing.</span></span> <span data-ttu-id="8d5a4-110">監査されるアクティビティについては、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8d5a4-110">To learn what activities are audited, see:</span></span>
    1. [<span data-ttu-id="8d5a4-111">ファイル アクティビティ</span><span class="sxs-lookup"><span data-stu-id="8d5a4-111">File activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#file-and-page-activities)
    1. [<span data-ttu-id="8d5a4-112">フォルダー アクティビティ</span><span class="sxs-lookup"><span data-stu-id="8d5a4-112">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    1. <span data-ttu-id="8d5a4-113">[共有アクティビティとアクセス アクティビティ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)。</span><span class="sxs-lookup"><span data-stu-id="8d5a4-113">[Sharing and Access activities](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities).</span></span>
1. <span data-ttu-id="8d5a4-114">サービスごとのすべての監査済みアクティビティのリストについては、「[監査済みアクティビティ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8d5a4-114">For a list of all audited activities by service, see [Audited activities](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).</span></span>
