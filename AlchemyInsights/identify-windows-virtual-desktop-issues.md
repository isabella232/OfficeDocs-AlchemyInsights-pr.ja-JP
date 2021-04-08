---
title: Windows Virtual Desktop の問題を特定する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596096"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="f3275-102">Windows Virtual Desktop の問題を特定する</span><span class="sxs-lookup"><span data-stu-id="f3275-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="f3275-103">Windows Virtual Desktop の診断では、1 つの Powershell コマンドレットを使用しますが、オプションのパラメータを多数含み、問題を絞り込んで特定します。</span><span class="sxs-lookup"><span data-stu-id="f3275-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="f3275-104">開始するには、</span><span class="sxs-lookup"><span data-stu-id="f3275-104">To get started:</span></span> 

1. <span data-ttu-id="f3275-105">Windows Virtual Desktop PowerShell モジュールをダウンロードしてインポートします。</span><span class="sxs-lookup"><span data-stu-id="f3275-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="f3275-106">詳細については、「[Windows PowerShell の Windows Virtual Desktop コマンドレット](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3275-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="f3275-107">次のコマンドレットを実行して、アカウントにサインインします。</span><span class="sxs-lookup"><span data-stu-id="f3275-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="f3275-108">例: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="f3275-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="f3275-109">**注意:** PowerShell を使用するすべてのクエリは、-UserName または -ActivityID パラメーターのいずれかを含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="f3275-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="f3275-110">監視機能の詳細については、「[診断機能の Log Analytics](https://go.microsoft.com/fwlink/?linkid=2126847) を使用する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3275-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="f3275-111">ユーザー別に診断アクティビティをフィルター処理するには、次のコマンドレットを実行します。</span><span class="sxs-lookup"><span data-stu-id="f3275-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="f3275-112">例: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="f3275-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="f3275-113">問題を診断するのに実行するフィルターの一覧です。</span><span class="sxs-lookup"><span data-stu-id="f3275-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="f3275-114">問題の診断の詳細については、「[Windows Virtual Desktop の問題を特定して診断する](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3275-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="f3275-115">一般的なエラーの詳細については、「[一般的なエラーのシナリオ](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3275-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
