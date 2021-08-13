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
ms.openlocfilehash: d0658b05b81ac45e7ce80323ad29898599482c4d3430d886627af6e9f8d136f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53985222"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>オンプレミスのフェデレーション サービス証明書のいずれかがまもなく期限切れになります

この問題を解決するには、次の手順を行います。
  
- コンピューター上で Windows PowerShell 用 Microsoft Azure Active Directory モジュールをインストールします (モジュールがまだインストールされていない場合)。これを行うには、「[Azure Active Directory PowerShell for Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)」 (Graph 用 Azure Active Directory PowerShell) に移動します。
    
- [フェデレーション ユーザーが Microsoft 365、Azure、または Intune にサインインするときに、AD FS から示された「サイトへのアクセスに関する問題が発生しました」エラー](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)の「シナリオ 1: AD FS トークン署名の証明書が失効している」セクションの手順に従います。
    
- 「[Microsoft 365、Azure、または Intune のフェデレーション ドメインの設定を更新または修復する方法](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)」の手順に従います。
    
フェデレーション証明書の更新に関する詳細については、[Office 365 および Azure AD 用の証明書の更新](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)に関するページを参照してください。
  

