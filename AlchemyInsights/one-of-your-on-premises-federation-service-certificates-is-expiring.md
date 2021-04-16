---
title: オンプレミスのフェデレーション サービス証明書のいずれかがまもなく期限切れになります
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 45a679e83aa8f07d65d2e7e84d7eb2a2b5a721e8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810057"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="fc50f-102">オンプレミスのフェデレーション サービス証明書のいずれかがまもなく期限切れになります</span><span class="sxs-lookup"><span data-stu-id="fc50f-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="fc50f-103">この問題を解決するには、次の手順を行います。</span><span class="sxs-lookup"><span data-stu-id="fc50f-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="fc50f-p101">コンピューター上で Windows PowerShell 用 Microsoft Azure Active Directory モジュールをインストールします (モジュールがまだインストールされていない場合)。これを行うには、「[Azure Active Directory PowerShell for Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)」 (Graph 用 Azure Active Directory PowerShell) に移動します。</span><span class="sxs-lookup"><span data-stu-id="fc50f-p101">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed). To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="fc50f-106">[フェデレーション ユーザーが Microsoft 365、Azure、または Intune にサインインするときに、AD FS から示された「サイトへのアクセスに関する問題が発生しました」エラー](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)の「シナリオ 1: AD FS トークン署名の証明書が失効している」セクションの手順に従います。</span><span class="sxs-lookup"><span data-stu-id="fc50f-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="fc50f-107">「[Microsoft 365、Azure、または Intune のフェデレーション ドメインの設定を更新または修復する方法](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)」の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="fc50f-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="fc50f-108">フェデレーション証明書の更新に関する詳細については、[Office 365 および Azure AD 用の証明書の更新](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="fc50f-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

