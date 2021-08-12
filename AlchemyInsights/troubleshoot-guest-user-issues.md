---
title: ゲスト ユーザーに関する問題のトラブルシューティング
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939384"
---
# <a name="troubleshoot-guest-user-issues"></a>ゲスト ユーザーに関する問題のトラブルシューティング

1. アプリケーションへのゲストアクセスの管理に関するガイダンスについては、「[Azure AD のアクセス レビューによるゲスト アクセスの管理](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)」を参照してください。
1. [Azure portal のディレクトリにゲストユーザーを追加する](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): このクイックスタートでは、Azure portal を介して新しいゲストユーザーを Azure AD ディレクトリに追加し、招待状を送信して、ゲストユーザーの招待状の引き換えプロセスがどのようになるかを確認します。
1. [PowerShell を使用してゲストユーザーを追加する](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): このクイックスタートでは、New-AzureADMSInvitation コマンドを使用して、1 人のゲストユーザーを Azure テナントに追加します。
1. Azure ポータル内からまたは PowerShell を使用して、Azure Active Directory (Azure AD) のエンタープライズ アプリケーションにユーザーとグループを割り当てる方法については、「[Azure Active Directory でのアプリのユーザー割り当ての管理](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)」を参照してください。 
1. Azure Active Directory (Azure AD) B2B コラボレーションは、Azure ADと統合するほとんどのアプリで機能します。 この[記事](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)では、Azure AD B2B で使用するためにいくつかの一般的な SaaS アプリを構成する手順について説明します。
1. Azure Active Directory (Azure AD) B2B コラボレーション機能を使用してパートナー組織からゲストユーザーを Azure AD に招待する組織として、これらの B2B ユーザーにオンプレミス アプリへのアクセスを提供できるようになりました。 これらのオンプレミス アプリは、SAML ベースの認証または Kerberos 制約付き委任 (KCD) を使用した統合 Windows 認証 (IWA) を使用できます。 詳細については、「[Azure AD の B2B ユーザーにオンプレミスのアプリケーションへのアクセスを許可する](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)」をご覧ください。
1. [Azure AD B2B コラボレーションを使用して、ローカルで管理されているパートナー アカウントにクラウド リソースへのアクセスを許可する](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)方法を確認してください。