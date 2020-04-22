---
title: ADFS フェデレーション証明書の期限切れ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710412"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="bce25-102">ADFS フェデレーション証明書の期限切れ</span><span class="sxs-lookup"><span data-stu-id="bce25-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="bce25-103">この問題を解決するには、次の手順を行います。</span><span class="sxs-lookup"><span data-stu-id="bce25-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="bce25-p101">コンピューター上で Windows PowerShell 用 Microsoft Azure Active Directory モジュールをインストールします (モジュールがまだインストールされていない場合)。これを行うには、[Windows PowerShell を使用した Azure AD の管理](https://aka.ms/aadposh)に関するページに移動します。</span><span class="sxs-lookup"><span data-stu-id="bce25-p101">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed). To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="bce25-106">[フェデレーションユーザーが Microsoft 365、Azure、または Intune に](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)サインインすると、「シナリオ 1: ad fs トークン署名証明書の有効期限が切れています。」の手順を実行して、ad fs の "サイトにアクセス中に問題が発生しました" というセクションの手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="bce25-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="bce25-107">[「Microsoft、Azure、または Intune のフェデレーションドメインの設定を更新または修復](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)する」の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="bce25-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="bce25-108">フェデレーション証明書の更新の詳細については、「 [Microsoft 365 および Azure Active Directory のフェデレーション証明書を更新](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bce25-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
