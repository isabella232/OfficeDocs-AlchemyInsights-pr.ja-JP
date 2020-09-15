---
title: ADFS フェデレーション証明書の期限切れ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686719"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="9d2f3-102">ADFS フェデレーション証明書の期限切れ</span><span class="sxs-lookup"><span data-stu-id="9d2f3-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="9d2f3-103">この問題を解決するには、次の手順を行います。</span><span class="sxs-lookup"><span data-stu-id="9d2f3-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="9d2f3-p101">コンピューター上で Windows PowerShell 用 Microsoft Azure Active Directory モジュールをインストールします (モジュールがまだインストールされていない場合)。これを行うには、[Windows PowerShell を使用した Azure AD の管理](https://aka.ms/aadposh)に関するページに移動します。</span><span class="sxs-lookup"><span data-stu-id="9d2f3-p101">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed). To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="9d2f3-106">[フェデレーション ユーザーが Microsoft 365、Azure、または Intune にサインインするときに、AD FS から示された「サイトへのアクセスに関する問題が発生しました」エラー](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)の「シナリオ 1: AD FS トークン署名の証明書が失効している」セクションの手順に従います。</span><span class="sxs-lookup"><span data-stu-id="9d2f3-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="9d2f3-107">「[Microsoft、Azure、または Intune のフェデレーション ドメインの設定を更新または修復する](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)」の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="9d2f3-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="9d2f3-108">フェデレーション証明書の更新に関する詳細については、「[Microsoft 365 および Azure Active Directory 用のフェデレーション証明書の更新](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9d2f3-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
