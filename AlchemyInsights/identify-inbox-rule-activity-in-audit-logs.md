---
title: 監査ログで受信トレイルールのアクティビティを識別する
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 51c25897223371a6dcc94c948955107ce74b0e8e
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383030"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="ccaca-102">監査ログで受信トレイルールのアクティビティを識別する</span><span class="sxs-lookup"><span data-stu-id="ccaca-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="ccaca-103">セキュリティ & コンプライアンスセンターで監査ログの検索を使用して、受信トレイルールのイベント (受信トレイルールの作成、変更、および削除) を表示できます。</span><span class="sxs-lookup"><span data-stu-id="ccaca-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="ccaca-104">[Office 365 セキュリティ & コンプライアンスセンター](https://protection.office.com/)にログインする</span><span class="sxs-lookup"><span data-stu-id="ccaca-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="ccaca-105">[**検索と調査**] をクリックして、[**監査ログの検索**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="ccaca-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="ccaca-106">[**開始日**] フィールドと [**終了日**] フィールドで日付範囲を選択します。</span><span class="sxs-lookup"><span data-stu-id="ccaca-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="ccaca-107">[ **Exchange メールボックスアクティビティ**] で、[**アクティビティ**] フィールドが [**新規-受信トレイルールの作成/変更/有効化/有効化/無効化**] に設定されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="ccaca-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="ccaca-108">**[検索]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="ccaca-108">Click **Search**.</span></span>

<span data-ttu-id="ccaca-109">結果から、監査レコードを選択します。</span><span class="sxs-lookup"><span data-stu-id="ccaca-109">In the results, select an audit record.</span></span> <span data-ttu-id="ccaca-110">詳細ポップアップで、[**詳細情報**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="ccaca-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="ccaca-111">受信トレイルールの設定に関する情報は、[**パラメーター** ] フィールドに表示されます。</span><span class="sxs-lookup"><span data-stu-id="ccaca-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="ccaca-112">詳細については、「[ユーザーが受信トレイルールを作成したか](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)どうかの判断」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ccaca-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
