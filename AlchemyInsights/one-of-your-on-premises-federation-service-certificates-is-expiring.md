---
title: 設置、フェデレーション サービスの証明書のいずれかが期限切れにします。
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
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 9e2e1a1dd2993b2a02b4405db8a707b23ff4af16
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29658912"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="4b55b-102">設置、フェデレーション サービスの証明書のいずれかが期限切れにします。</span><span class="sxs-lookup"><span data-stu-id="4b55b-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="4b55b-103">この問題を解決するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="4b55b-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="4b55b-p101">(モジュールがまだインストールされていない) 場合は、コンピューターに、Microsoft Azure Active Directory モジュールの Windows PowerShell をインストールします。[グラフのアクティブなディレクトリの PowerShell を Azure](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)にはこれを行うには、</span><span class="sxs-lookup"><span data-stu-id="4b55b-p101">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed). To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="4b55b-106">手順に従います、「シナリオ 1: AD FS トークン署名証明書の有効期限が切れて」[から AD FS のフェデレーション ユーザーが Office 365 Azure Intune にサインインするときの「サイトへアクセス問題が発生しました」エラー](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)のセクション。</span><span class="sxs-lookup"><span data-stu-id="4b55b-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="4b55b-107">T[を更新または、Office 365、Azure、Intune のフェデレーション ドメインの設定を修復する方法](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="4b55b-107">Follow the steps in t[How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="4b55b-108">フェデレーション証明書の更新の詳細については、 [O365 と Azure AD の証明書の更新](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4b55b-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

