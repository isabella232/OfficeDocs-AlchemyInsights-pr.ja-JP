---
title: SharePoint および OneDrive のアラートの受信の遅延
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 02/04/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 0bc9f614047e06e8654a9b3ff64e87427f33139f
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/04/2020
ms.locfileid: "41771220"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="a39f8-102">SharePoint および OneDrive のアラートの受信の遅延</span><span class="sxs-lookup"><span data-stu-id="a39f8-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="a39f8-103">まずは、メールの迷惑メール フォルダーまたはスパム フォルダーを確認します。</span><span class="sxs-lookup"><span data-stu-id="a39f8-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="a39f8-104">**複数のファイルまたはライブラリからのすべてのアラートの配信に遅延がある**場合は、[サービス正常性ダッシュボード](https://nam06.safelinks.protection.outlook.com/?url=https://admin.microsoft.com/AdminPortal/Home%23/servicehealth&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0)にアクセスして SharePoint または Exchange で発生している可能性のあるアドバイザリやインシデントを確認します。</span><span class="sxs-lookup"><span data-stu-id="a39f8-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://nam06.safelinks.protection.outlook.com/?url=https://admin.microsoft.com/AdminPortal/Home%23/servicehealth&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="a39f8-105">問題は、SharePoint のアラート機能または Exchange を介したメールの遅延にある可能性があります。</span><span class="sxs-lookup"><span data-stu-id="a39f8-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="a39f8-106">また、他のメールが配信されているかどうかにも注意してください。もしも配信されていない場合には、おそらく問題は Exchange の遅延にあります。</span><span class="sxs-lookup"><span data-stu-id="a39f8-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="a39f8-107">**特定のファイルまたはライブラリからの個別のアラートが配信されない**場合には、削除して再作成してみてください。</span><span class="sxs-lookup"><span data-stu-id="a39f8-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="a39f8-108">詳細については、「[SharePoint アラートの管理、表示、または削除](https://nam06.safelinks.protection.outlook.com/?url=https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax/epn3E%3D&reserved=0)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a39f8-108">See [Manage, view, or delete SharePoint alerts](https://nam06.safelinks.protection.outlook.com/?url=https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax/epn3E%3D&reserved=0) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="a39f8-109">アラートを配布グループに送信することはできません。</span><span class="sxs-lookup"><span data-stu-id="a39f8-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="a39f8-110">セキュリティおよび O365 グループのみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="a39f8-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="a39f8-111">アラートのメール テンプレートをカスタマイズすることはできません。</span><span class="sxs-lookup"><span data-stu-id="a39f8-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="a39f8-112">これらを実現するには、Microsoft Flow または SharePoint Designer ワークフローを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a39f8-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
