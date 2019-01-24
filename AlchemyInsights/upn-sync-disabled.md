---
title: UPN の同期が無効になっています。
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: d00f10688ec775c22d60a9089e291c265ada46f1
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29477042"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="21f3e-102">UPN の同期が無効になっています。</span><span class="sxs-lookup"><span data-stu-id="21f3e-102">UPN sync disabled</span></span>

<span data-ttu-id="21f3e-103">2016 年 3 月 30 日前に AD を Azure に同期を開始する場合は、UPN ソフト一致する組織のみを有効にするのには、次の Azure AD の PowerShell コマンドレットを実行します。</span><span class="sxs-lookup"><span data-stu-id="21f3e-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="21f3e-104">**セット-MsolDirSyncFeature-EnableSoftMatchOnUpn をフィーチャー-$True を有効にします。**</span><span class="sxs-lookup"><span data-stu-id="21f3e-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="21f3e-105">ソフト一致の UPN が自動的に有効に 2016 年 3 月 30 日以降に、Azure AD への同期を開始する組織です。</span><span class="sxs-lookup"><span data-stu-id="21f3e-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="21f3e-106">ソフト一致 UPN およびその他の同期機能を有効にする方法については、 [Azure AD 接続の同期サービスの機能](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="21f3e-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

