---
title: ADFS フェデレーション証明書の期限切れ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 55529265d2356a911624026107fb639f93e29abd
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "29925385"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="fa618-102">ADFS フェデレーション証明書の期限切れ</span><span class="sxs-lookup"><span data-stu-id="fa618-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="fa618-103">この問題を解決するには、次の手順を行います。</span><span class="sxs-lookup"><span data-stu-id="fa618-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="fa618-p101">コンピューター上で Windows PowerShell 用 Microsoft Azure Active Directory モジュールをインストールします (モジュールがまだインストールされていない場合)。これを行うには、[Windows PowerShell を使用した Azure AD の管理](https://aka.ms/aadposh)に関するページに移動します。</span><span class="sxs-lookup"><span data-stu-id="fa618-p101">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed). To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>
    
2. <span data-ttu-id="fa618-106">[フェデレーション ユーザーが Office 365、Azure、または Intune にサインインするときに、AD FS から示された "サイトへのアクセスに関する問題が発生しました " エラー](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)の "シナリオ 1: AD FS トークン署名の証明書が失効している" セクションの手順に従います。</span><span class="sxs-lookup"><span data-stu-id="fa618-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
3. <span data-ttu-id="fa618-107">「[Office 365、Azure、または Intune のフェデレーション ドメインの設定を更新または修復する方法](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)」の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="fa618-107">Follow the steps in [How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
    <span data-ttu-id="fa618-108">フェデレーション証明書の更新に関する詳細については、「[Office 365 および Azure Active Directory 用のフェデレーション証明書の更新](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fa618-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
    

