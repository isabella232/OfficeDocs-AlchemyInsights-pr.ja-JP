---
title: 監査ログで受信トレイのルール アクティビティを特定する
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779056"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="95eb2-102">監査ログで受信トレイのルール アクティビティを特定する</span><span class="sxs-lookup"><span data-stu-id="95eb2-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="95eb2-103">Microsoft 365 セキュリティ/コンプライアンス センターで、監査ログの検索を使用して、受信トレイのルールのイベント (受信トレイのルールの作成、変更、および削除) を表示することができます。</span><span class="sxs-lookup"><span data-stu-id="95eb2-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="95eb2-104">[Microsoft 365 セキュリティ/コンプライアンス センター](https://protection.office.com/)にログインします。</span><span class="sxs-lookup"><span data-stu-id="95eb2-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="95eb2-105">**[検索]** > **[監査ログの検索]** ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="95eb2-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="95eb2-106">[**開始日**] と [**終了日**] フィールドで日付範囲を選択します。</span><span class="sxs-lookup"><span data-stu-id="95eb2-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="95eb2-107">[**Exchange メールボックスのアクティビティ**] の下で、[**アクティビティ**] フィールドが [**New-InboxRule 受信トレイのルールの作成/変更/有効化/無効化**] に設定されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="95eb2-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="95eb2-108">[**検索**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="95eb2-108">Click **Search**.</span></span>

<span data-ttu-id="95eb2-109">結果から、[監査レコード] を選択します。</span><span class="sxs-lookup"><span data-stu-id="95eb2-109">In the results, select an audit record.</span></span> <span data-ttu-id="95eb2-110">詳細ポップアップから、 [**詳細情報**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="95eb2-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="95eb2-111">受信トレイのルール設定に関する情報は、[**パラメーター**] フィールドに表示されます。</span><span class="sxs-lookup"><span data-stu-id="95eb2-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="95eb2-112">詳細については、「[ユーザーが受信トレイ ルールを作成したかどうかを判別する](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="95eb2-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
