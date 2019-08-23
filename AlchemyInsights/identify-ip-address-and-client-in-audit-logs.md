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
ms.openlocfilehash: e0119762d2a34bd2b0da827faf55c832e29d8a2b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539034"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="ee0d0-102">監査ログで IP アドレスとクライアントを識別する</span><span class="sxs-lookup"><span data-stu-id="ee0d0-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="ee0d0-103">Office 365 ユーザーまたは管理者によってアクティビティに対応する IP アドレスが監査ログに表示されます。</span><span class="sxs-lookup"><span data-stu-id="ee0d0-103">The IP address that corresponds to an activity by an Office 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="ee0d0-104">クライアント情報も記録されます。</span><span class="sxs-lookup"><span data-stu-id="ee0d0-104">The client information is also logged.</span></span> <span data-ttu-id="ee0d0-105">このような情報を識別する手順は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="ee0d0-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="ee0d0-106">[Office 365 セキュリティ & コンプライアンスセンター](https://protection.office.com/)にログインします。</span><span class="sxs-lookup"><span data-stu-id="ee0d0-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="ee0d0-107">[ \*\*\*\* > **監査ログ**の検索] ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="ee0d0-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="ee0d0-108">特定のアクティビティに関心がある場合は、[**アクティビティ**] リストから選択します。</span><span class="sxs-lookup"><span data-stu-id="ee0d0-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="ee0d0-109">指定しない場合は、選択したユーザーに対してすべてのアクティビティが返されます (既定の設定)。</span><span class="sxs-lookup"><span data-stu-id="ee0d0-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="ee0d0-110">**注**: 特定のアクティビティが [**操作**] メニューに表示されない場合があります。ただし、[**すべてのアクティビティの結果を表示する]** が選択されている場合は、これらの監査アイテムが返されます (既定の設定)。</span><span class="sxs-lookup"><span data-stu-id="ee0d0-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="ee0d0-111">[**ユーザー** ] フィールドでユーザー名を指定し、アクティビティに該当する日付の範囲を選択して、[**検索**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="ee0d0-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="ee0d0-112">結果には、そのアクティビティの IP アドレスが結果ウィンドウに表示されます。</span><span class="sxs-lookup"><span data-stu-id="ee0d0-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="ee0d0-113">監査レコードを選択して、**詳細**ポップアップ (たとえば、[クライアント]、[アクションを実行したユーザー] など) で詳細情報を表示します。</span><span class="sxs-lookup"><span data-stu-id="ee0d0-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="ee0d0-114">詳細については、「[危害を受けたアカウントへのアクセスに使用されたコンピューターの IP アドレスを検索する](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ee0d0-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
