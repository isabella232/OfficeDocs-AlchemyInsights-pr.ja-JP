---
title: SharePoint および OneDrive のアラートを受信しない
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/25/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 80423791ad558fc414d50608c73f823036432e14
ms.sourcegitcommit: 5e6a805fb0b41d714ca1cf90e23b8e2daa90f90e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/26/2019
ms.locfileid: "37313934"
---
# <a name="not-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="f3589-102">SharePoint および OneDrive のアラートを受信しない</span><span class="sxs-lookup"><span data-stu-id="f3589-102">Not receiving SharePoint and OneDrive alerts</span></span>

<span data-ttu-id="f3589-103">まずは、メールの迷惑メール フォルダーまたはスパム フォルダーを確認します。</span><span class="sxs-lookup"><span data-stu-id="f3589-103">First check the Junk or Spam folder in your email.</span></span>

<span data-ttu-id="f3589-104">次に、**すべてのアラートが配信されていない**のか、それとも特定のファイルまたはライブラリからの**個別のアラート**が配信されていないのかを判断します。</span><span class="sxs-lookup"><span data-stu-id="f3589-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="f3589-105">**複数のファイルまたはライブラリからのすべてのアラートが配信されていない**場合は、[サービス正常性ダッシュボード](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fadmin.microsoft.com%2FAdminPortal%2FHome%23%2Fservicehealth&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0)にアクセスして SharePoint または Exchange で発生している可能性のあるアドバイザリやインシデントを確認します。</span><span class="sxs-lookup"><span data-stu-id="f3589-105">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fadmin.microsoft.com%2FAdminPortal%2FHome%23%2Fservicehealth&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="f3589-106">問題は、SharePoint のアラート機能または Exchange を介したメールの遅延にある可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f3589-106">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="f3589-107">また、他のメールが配信されているかどうかにも注意してください。もしも配信されていない場合には、おそらく問題は Exchange の遅延にあります。</span><span class="sxs-lookup"><span data-stu-id="f3589-107">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="f3589-108">**特定のファイルまたはライブラリからの個別のアラートが配信されない**場合には、削除して再作成してみてください。</span><span class="sxs-lookup"><span data-stu-id="f3589-108">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="f3589-109">詳細については、「[SharePoint アラートの管理、表示、または削除](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2Fmanage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2%3Fui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax%2Fepn3E%3D&reserved=0)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3589-109">See [Manage, view, or delete SharePoint alerts](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2Fmanage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2%3Fui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax%2Fepn3E%3D&reserved=0) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="f3589-110">アラートを配布グループに送信することはできません。</span><span class="sxs-lookup"><span data-stu-id="f3589-110">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="f3589-111">セキュリティおよび O365 グループのみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f3589-111">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="f3589-112">アラートのメール テンプレートをカスタマイズすることはできません。</span><span class="sxs-lookup"><span data-stu-id="f3589-112">You cannot customize alert email templates.</span></span> <span data-ttu-id="f3589-113">これらを実現するには、Microsoft Flow または SharePoint Designer ワークフローを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f3589-113">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
