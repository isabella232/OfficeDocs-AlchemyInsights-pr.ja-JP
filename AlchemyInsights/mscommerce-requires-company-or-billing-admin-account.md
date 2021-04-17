---
title: MSCommerce モジュールに接続する
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3529"
ms.openlocfilehash: 8e6819f6d6ff37baab4bdd49cb5a87c32490f841
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51829741"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a><span data-ttu-id="5ed9b-102">MSCommerce には、会社または課金管理者アカウントが必要です</span><span class="sxs-lookup"><span data-stu-id="5ed9b-102">MSCommerce requires a Company or Billing Administrator account</span></span>

<span data-ttu-id="5ed9b-103">MSCommerce モジュールには、会社または課金管理者の特権を持つアカウントが必要です。</span><span class="sxs-lookup"><span data-stu-id="5ed9b-103">The MSCommerce module requires an account with Company or Billing Administrator privileges.</span></span> <span data-ttu-id="5ed9b-104">次のエラーが表示される場合は、別のアカウントで再接続する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5ed9b-104">If you are receiving the following error, you will need to reconnect with a different account.</span></span>

<span data-ttu-id="5ed9b-105">*ErrorMessage - リモート サーバーがエラーを返しました: (403) 禁止されています。ErrorDetails - C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*</span><span class="sxs-lookup"><span data-stu-id="5ed9b-105">*ErrorMessage - The remote server returned an error: (403) Forbidden. ErrorDetails - At C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*</span></span><br>
<span data-ttu-id="5ed9b-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Failed to retri ...*</span><span class="sxs-lookup"><span data-stu-id="5ed9b-106">*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Failed to retri ...*</span></span><br>
<span data-ttu-id="5ed9b-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span><span class="sxs-lookup"><span data-stu-id="5ed9b-107">\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~</span></span><br>
<span data-ttu-id="5ed9b-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo          : NotSpecified: (:) [Write-Error], WriteErrorException*</span><span class="sxs-lookup"><span data-stu-id="5ed9b-108">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo          : NotSpecified: (:) [Write-Error], WriteErrorException*</span></span><br>
<span data-ttu-id="5ed9b-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*</span><span class="sxs-lookup"><span data-stu-id="5ed9b-109">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*</span></span>

<span data-ttu-id="5ed9b-110">アカウントに会社または課金管理者の特権がない場合は、IT 管理者にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="5ed9b-110">If your account does not have Company or Billing Administrator privileges, contact your IT Admin.</span></span>
