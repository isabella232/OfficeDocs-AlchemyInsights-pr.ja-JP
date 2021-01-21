---
title: LDAP の構成
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885815"
---
# <a name="configure-ldap"></a><span data-ttu-id="d1cb9-102">LDAP の構成</span><span class="sxs-lookup"><span data-stu-id="d1cb9-102">Configure LDAP</span></span>

<span data-ttu-id="d1cb9-103">LDAP を構成するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="d1cb9-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="d1cb9-104">[Azure portal](https://aka.ms/aadds-health) でドメインの正常性を確認します。</span><span class="sxs-lookup"><span data-stu-id="d1cb9-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="d1cb9-105">有効な Azure AD サブスクリプションが使用可能であり、Azure AD Domain Services が有効になっていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="d1cb9-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="d1cb9-106">セキュア LDAP を有効にするために必要な証明書は、信頼できる公開証明機関から取得するか、または自己署名証明書である必要があります。</span><span class="sxs-lookup"><span data-stu-id="d1cb9-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="d1cb9-107">証明書が必要な[ガイドライン](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)に従っていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="d1cb9-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="d1cb9-108">**証明書が無効です**</span><span class="sxs-lookup"><span data-stu-id="d1cb9-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="d1cb9-109">証明書を更新するには、「[LDAP の構成](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)」の手順に従って新しい証明書を作成し、再アップロードします。</span><span class="sxs-lookup"><span data-stu-id="d1cb9-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="d1cb9-110">Azure Active Directory Domain Services のセキュア LDAP アラートの既知の問題を解決するには、「[LDAP アラートの解決](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d1cb9-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
