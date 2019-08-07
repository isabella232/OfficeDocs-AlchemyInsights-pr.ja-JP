---
title: 監査ログで IP アドレスとクライアントを識別する
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: a91778c006531371b85116f5c97485d42e6cc5be
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35382958"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="74220-102">監査ログで IP アドレスとクライアントを識別する</span><span class="sxs-lookup"><span data-stu-id="74220-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="74220-103">監査ログには、ユーザーまたは管理者によるアクティビティに対応する IP アドレスが表示されます。</span><span class="sxs-lookup"><span data-stu-id="74220-103">The IP address that corresponds to an activity by a user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="74220-104">クライアント情報も記録されます。</span><span class="sxs-lookup"><span data-stu-id="74220-104">The client information is also logged.</span></span> <span data-ttu-id="74220-105">ここでは、そのような情報を識別するための手順をご紹介します。</span><span class="sxs-lookup"><span data-stu-id="74220-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="74220-106">[Office 365  セキュリティ/コンプライアンス センター](https://protection.office.com/)にログインする</span><span class="sxs-lookup"><span data-stu-id="74220-106">[Search the audit log in the Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="74220-107">[**検索と調査**] と [**監査ログ検索**]をクリックする。</span><span class="sxs-lookup"><span data-stu-id="74220-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

   <span data-ttu-id="74220-108">特定のアクティビティに関心があるなら、[**アクティビティ**] リストから選択します。</span><span class="sxs-lookup"><span data-stu-id="74220-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="74220-109">そうでない場合は、選択したユーザーのすべての活動が返されます(既定の設定) 。</span><span class="sxs-lookup"><span data-stu-id="74220-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="74220-110">**注意**: 特定のアクティビティは、[**アクティビティ**] のメニューに表示されない場合があります。ただし、[**すべてのアクティビティの結果を表示**] が選択されていれば、これらの監査項目が返されます（デフォルト設定）。</span><span class="sxs-lookup"><span data-stu-id="74220-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="74220-111">[**ユーザー**] フィールド内のユーザー名を指定し、アクティビティの適切な日付の範囲を選択し、[**検索**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="74220-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="74220-112">結果では、結果ウィンドウでそのアクティビティの IP アドレスを見ることができます。</span><span class="sxs-lookup"><span data-stu-id="74220-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="74220-113">[**詳細情報**] ポップアップにある [監査記録] を選択し、 詳細な情報 (たとえば、クライアント、アクションを実行したユーザーなど)を表示します。</span><span class="sxs-lookup"><span data-stu-id="74220-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="74220-114">詳細については [安全性が脅かされたアカウントへのアクセスに使用されたコンピューターの IP アドレスを見つける](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="74220-114">Finding the IP address of the computer used to access a compromised account</span></span>
