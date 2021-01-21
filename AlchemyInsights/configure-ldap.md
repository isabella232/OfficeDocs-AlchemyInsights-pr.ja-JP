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
# <a name="configure-ldap"></a>LDAP の構成

LDAP を構成するには、次の手順を実行します。

1. [Azure portal](https://aka.ms/aadds-health) でドメインの正常性を確認します。
1. 有効な Azure AD サブスクリプションが使用可能であり、Azure AD Domain Services が有効になっていることを確認します。
1. セキュア LDAP を有効にするために必要な証明書は、信頼できる公開証明機関から取得するか、または自己署名証明書である必要があります。
1. 証明書が必要な[ガイドライン](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)に従っていることを確認してください。

**証明書が無効です**
1. 証明書を更新するには、「[LDAP の構成](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)」の手順に従って新しい証明書を作成し、再アップロードします。
1. Azure Active Directory Domain Services のセキュア LDAP アラートの既知の問題を解決するには、「[LDAP アラートの解決](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)」を参照してください。
