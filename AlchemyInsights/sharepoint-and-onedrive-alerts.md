---
title: SharePoint および OneDrive 通知を受信しない
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
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/26/2019
ms.locfileid: "37313934"
---
# <a name="not-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="20f9f-102">SharePoint および OneDrive 通知を受信しない</span><span class="sxs-lookup"><span data-stu-id="20f9f-102">Not receiving SharePoint and OneDrive alerts</span></span>

<span data-ttu-id="20f9f-103">まず、電子メールの [迷惑メール] フォルダーまたは [スパム] フォルダーをチェックします。</span><span class="sxs-lookup"><span data-stu-id="20f9f-103">First check the Junk or Spam folder in your email.</span></span>

<span data-ttu-id="20f9f-104">次に、**すべての通知が配信されてい**ないか、特定のファイルまたはライブラリからの**個々の通知**が配信されていないかを確認します。</span><span class="sxs-lookup"><span data-stu-id="20f9f-104">Then determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="20f9f-105">**複数のファイルまたはライブラリからのすべての通知が配信**されない場合は、[サービス正常性ダッシュボード](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fadmin.microsoft.com%2FAdminPortal%2FHome%23%2Fservicehealth&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0)にアクセスして、SharePoint または Exchange で発生している可能性があるすべてのアドバイザリ/インシデントをチェックします。</span><span class="sxs-lookup"><span data-stu-id="20f9f-105">If **all alerts from multiple files or libraries are not delivered**, visit the [Service Health dashboard](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fadmin.microsoft.com%2FAdminPortal%2FHome%23%2Fservicehealth&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="20f9f-106">この問題は、Exchange による電子メールの SharePoint 通知機能または遅延が原因である可能性があります。</span><span class="sxs-lookup"><span data-stu-id="20f9f-106">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="20f9f-107">また、他のメールが配信されているかどうかにも注意してください。そうでない場合は、Exchange の遅延が原因である可能性があります。</span><span class="sxs-lookup"><span data-stu-id="20f9f-107">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="20f9f-108">**特定のファイルまたはライブラリからの個々の通知が配信されない**場合は、削除して再作成します。</span><span class="sxs-lookup"><span data-stu-id="20f9f-108">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="20f9f-109">通知を再作成するには、「 [SharePoint alerts を管理、表示、または削除](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2Fmanage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2%3Fui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax%2Fepn3E%3D&reserved=0)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="20f9f-109">See [Manage, view, or delete SharePoint alerts](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2Fmanage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2%3Fui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax%2Fepn3E%3D&reserved=0) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="20f9f-110">通知を配布グループに送信することはできません。</span><span class="sxs-lookup"><span data-stu-id="20f9f-110">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="20f9f-111">セキュリティと O365 グループのみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="20f9f-111">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="20f9f-112">通知電子メールテンプレートをカスタマイズすることはできません。</span><span class="sxs-lookup"><span data-stu-id="20f9f-112">You cannot customize alert email templates.</span></span> <span data-ttu-id="20f9f-113">これらを実現するには、Microsoft Flow または SharePoint Designer ワークフローを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="20f9f-113">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
