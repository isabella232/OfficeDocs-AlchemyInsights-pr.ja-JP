---
title: 監査ログで IP アドレスとクライアントを識別する
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716393"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="8c4c2-102">監査ログで IP アドレスとクライアントを識別する</span><span class="sxs-lookup"><span data-stu-id="8c4c2-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="8c4c2-103">監査ログには、Microsoft 365 ユーザーまたは管理者によるアクティビティに対応する IP アドレスが表示されます。</span><span class="sxs-lookup"><span data-stu-id="8c4c2-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="8c4c2-104">クライアント情報も記録されます。</span><span class="sxs-lookup"><span data-stu-id="8c4c2-104">The client information is also logged.</span></span> <span data-ttu-id="8c4c2-105">ここでは、そのような情報を識別するための手順をご紹介します。</span><span class="sxs-lookup"><span data-stu-id="8c4c2-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="8c4c2-106">[Microsoft 365 セキュリティ/コンプライアンス センター](https://protection.office.com/) にログインします。</span><span class="sxs-lookup"><span data-stu-id="8c4c2-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="8c4c2-107">**[検索]** > **[監査ログの検索]** ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="8c4c2-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="8c4c2-108">特定のアクティビティに関心がある場合は、[**アクティビティ**] リストから選択します。</span><span class="sxs-lookup"><span data-stu-id="8c4c2-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="8c4c2-109">そうでない場合は、選択したユーザーのすべての活動が返されます(既定の設定) 。</span><span class="sxs-lookup"><span data-stu-id="8c4c2-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="8c4c2-110">**注意**: 特定のアクティビティは、[**アクティビティ**] のメニューに表示されない場合があります。ただし、[**すべてのアクティビティの結果を表示**] が選択されていれば、これらの監査項目が返されます（デフォルト設定）。</span><span class="sxs-lookup"><span data-stu-id="8c4c2-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="8c4c2-111">[**ユーザー**] フィールド内のユーザー名を指定し、アクティビティの適切な日付の範囲を選択し、[**検索**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="8c4c2-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="8c4c2-112">結果では、結果ウィンドウでそのアクティビティの IP アドレスを見ることができます。</span><span class="sxs-lookup"><span data-stu-id="8c4c2-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="8c4c2-113">[**詳細情報**] ポップアップにある [監査記録] を選択し、 詳細な情報 (たとえば、クライアント、アクションを実行したユーザーなど)を表示します。</span><span class="sxs-lookup"><span data-stu-id="8c4c2-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="8c4c2-114">詳細については [安全性が脅かされたアカウントへのアクセスに使用されたコンピューターの IP アドレスを見つける](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8c4c2-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
