---
title: 932 のアップグレード AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9add88a0e4a2590639cbfc546afdcdf5e6aa4886
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29477278"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="6f46c-102">アップグレード Azure AD 接続します。</span><span class="sxs-lookup"><span data-stu-id="6f46c-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="6f46c-p101">既定では、最新のバージョンを実行していることを確認するのに役立ちます、Azure の AD 接続の自動アップグレードが有効になります。自動アップグレードの設定を確認するには、Azure AD PowerShell で**Get ADSyncAutoUpgrade**コマンドレットを使用します。コマンドレットには、次の値のいずれかが返されます。</span><span class="sxs-lookup"><span data-stu-id="6f46c-p101">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version. To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell. The cmdlet will return one of following values:</span></span> 
  
- <span data-ttu-id="6f46c-106">**有効**: 自動アップグレードが有効になっています。</span><span class="sxs-lookup"><span data-stu-id="6f46c-106">**Enabled**: Automatic upgrade is enabled.</span></span> 
    
- <span data-ttu-id="6f46c-107">**無効になります**: 自動アップグレードが無効になります。</span><span class="sxs-lookup"><span data-stu-id="6f46c-107">**Disabled**: Automatic upgrade is disabled.</span></span> 
    
- <span data-ttu-id="6f46c-p102">**保留**: システムは、自動アップグレードを受ける資格が不要になった。この値を構成することはできません。システムで設定されています。</span><span class="sxs-lookup"><span data-stu-id="6f46c-p102">**Suspended**: The system is no longer eligible to receive automatic upgrades. You can't configure this value; it's set by the system.</span></span> 
    
<span data-ttu-id="6f46c-110">詳細については、[自動アップグレード](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6f46c-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>
  
<span data-ttu-id="6f46c-111">Azure AD 接続の最新バージョンをダウンロードするには[https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)です。</span><span class="sxs-lookup"><span data-stu-id="6f46c-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
  

