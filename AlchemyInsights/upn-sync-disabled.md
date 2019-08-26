---
title: UPN 同期が無効
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: f390d659b191fa4c44bd7c8acb32409cd3021489
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36532336"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="217a6-102">UPN 同期が無効</span><span class="sxs-lookup"><span data-stu-id="217a6-102">UPN sync disabled</span></span>

<span data-ttu-id="217a6-103">2016 年 3 月 30 日より前に Azure AD との同期を開始した場合は、次の Azure AD PowerShell コマンドレットを実行して、ご自分の組織に対してのみ UPN あいまい一致を有効にします。</span><span class="sxs-lookup"><span data-stu-id="217a6-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="217a6-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span><span class="sxs-lookup"><span data-stu-id="217a6-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="217a6-105">UPN あいまい一致は、2016 年 3 月 30 日以降に Azure AD との同期を開始した組織に対しては自動的に有効になります。</span><span class="sxs-lookup"><span data-stu-id="217a6-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="217a6-106">UPN やその他の同期機能であいまい一致を有効にする方法の詳細については、「[Azure AD Connect 同期サービスの機能](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="217a6-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

