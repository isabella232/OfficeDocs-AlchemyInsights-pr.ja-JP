---
title: Yammer のライセンスに関する問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657281"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="a893f-102">Yammer のライセンスに関する問題</span><span class="sxs-lookup"><span data-stu-id="a893f-102">Yammer licensing issues</span></span>

<span data-ttu-id="a893f-103">すべてのユーザーは Yammer Enterprise サービスを使用するためにライセンスが必要ですが、既定では、Yammer ではユーザーがサービスにアクセスするためのライセンスを持っている必要はありません。</span><span class="sxs-lookup"><span data-stu-id="a893f-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="a893f-104">管理者が Yammer ライセンスのない Microsoft 365 ユーザーをブロックするように設定を変更した場合、Yammer Enterprise のライセンスが割り当てられていないユーザーは、Yammer サービスにアクセスできません。</span><span class="sxs-lookup"><span data-stu-id="a893f-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="a893f-105">詳しくは、「[Office 365 で Yammer ユーザー ライセンスを管理する](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a893f-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="a893f-106">ライセンスがユーザーから削除されると、Yammer タイルは表示されなくなり、他のサービスではライセンスの削除を使って機能を非表示にする可能性があります。</span><span class="sxs-lookup"><span data-stu-id="a893f-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="a893f-107">その他の場合、機能は表示されますが、動作するにはライセンスの割り当てが必要になります。</span><span class="sxs-lookup"><span data-stu-id="a893f-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="a893f-108">**ユーザーのライセンスが更新されない**</span><span class="sxs-lookup"><span data-stu-id="a893f-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="a893f-109">ユーザーにライセンスが割り当てられているのに、依然として Yammer にアクセスできない場合があります。</span><span class="sxs-lookup"><span data-stu-id="a893f-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="a893f-110">多数のライセンスの割り当てが進行中の場合、遅延が発生する可能性が高くなります。</span><span class="sxs-lookup"><span data-stu-id="a893f-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="a893f-111">システムが非同期で実行されているために、Azure AD でライセンスが変更されても、Yammer ユーザーが同じ順序で更新されないことがあります。</span><span class="sxs-lookup"><span data-stu-id="a893f-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="a893f-112">ライセンス同期の問題を報告するサポート ケースを開く前に、最大 24 時間待ってください。</span><span class="sxs-lookup"><span data-stu-id="a893f-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="a893f-113">**ライセンスの一括割り当て**</span><span class="sxs-lookup"><span data-stu-id="a893f-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="a893f-114">ライセンスは、管理センターまたは PowerShell スクリプトを使って割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="a893f-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="a893f-115">詳細については、「[ユーザーにライセンスを割り当てる](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)」と「[Office 365 PowerShell を使用してライセンスをユーザー アカウントに割り当てる](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a893f-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="a893f-116">Microsoft サポートではスクリプトの作成についてのサポートは提供していませんが、Yammer ライセンスの割り当てに関するドキュメントはご利用いただけます。</span><span class="sxs-lookup"><span data-stu-id="a893f-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="a893f-117">詳細については、「[Windows PowerShell を使用して Yammer ライセンスを管理する](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a893f-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>