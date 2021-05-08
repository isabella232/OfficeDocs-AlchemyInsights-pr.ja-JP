---
title: Microsoft 365 アプリのアドインの展開
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/30/2021
ms.locfileid: "52125856"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="562f4-102">Microsoft 365 アプリのアドインの展開</span><span class="sxs-lookup"><span data-stu-id="562f4-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="562f4-103">一元展開は、組織内のユーザーおよびグループに Office アドインを展開するための推奨方法です。</span><span class="sxs-lookup"><span data-stu-id="562f4-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="562f4-104">アドインを展開するには、以下の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="562f4-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="562f4-105">**注**: Office のアドインを個別のユーザーとしてインストールするには、「[Office プログラムでアドインを表示、管理、インストールする](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="562f4-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="562f4-106">また、Office ストア アドインの個別取得が有効になっていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="562f4-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> 

1. <span data-ttu-id="562f4-107">一元展開を使用して、環境がアドインの展開の要件を満たしていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="562f4-107">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="562f4-108">詳細については、[要件](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="562f4-108">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="562f4-109">Microsoft 365 管理センターで [**設定**]  >  [**統合アプリ**]  >  [**アプリを取得**] の順に移動して、アドインを展開します。</span><span class="sxs-lookup"><span data-stu-id="562f4-109">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="562f4-110">注:</span><span class="sxs-lookup"><span data-stu-id="562f4-110">Notes:</span></span> 

- <span data-ttu-id="562f4-111">統合アプリでは、管理者がグローバル管理者または Exchange 管理者の権限を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="562f4-111">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="562f4-112">アドインを複数のユーザーに展開する場合は、個々のユーザーではなくグループを使用して割り当てを行うことをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="562f4-112">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="562f4-113">詳細については、「[Considerations when assigning an add-in to users and groups (アドインをユーザーとグループに割り当てる際の考慮事項)](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="562f4-113">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="562f4-114">一元展開は、ネストされたグループまたは親グループを持つグループのユーザーをサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="562f4-114">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="562f4-115">詳細については、「[ユーザまたはグループへの割り当て](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="562f4-115">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="562f4-116">ユーザーがサインインできるように、Microsoft 365 アプリ管理サービス (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') が有効になっていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="562f4-116">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="562f4-117">詳細については、「 [アプリのプロパティを構成する](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="562f4-117">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="562f4-118">統合アプリを使用したアドインの展開で問題が発生した場合は、[アドイン](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)を使用した展開をお試しください。</span><span class="sxs-lookup"><span data-stu-id="562f4-118">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="562f4-119">詳細については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="562f4-119">For more information, see:</span></span>

<span data-ttu-id="562f4-120">「[管理センターでアドインを展開する](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)」
「[管理センターでアドインを管理する](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)」
「[一元展開 PowerShell コマンドレットを使用してアドインを管理する](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)」
「[Microsoft 365 管理センターからの一元展開を使用した Microsoft アドインの発行](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)」
「[トラブルシューティング: ユーザーのアドインが表示されない](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)」
「[Office アドインでのユーザー エラーのトラブルシューティング](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)」</span><span class="sxs-lookup"><span data-stu-id="562f4-120">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>