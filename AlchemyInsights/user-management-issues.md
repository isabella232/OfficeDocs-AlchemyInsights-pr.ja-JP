---
title: ユーザー管理に関する問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2021
ms.locfileid: "51038299"
---
# <a name="user-management-issues"></a>ユーザー管理に関する問題

**[ユーザー割り当てが必要] を無効に(このプロパティを [いいえ] に設定)した場合、 アプリケーションに現在割り当てられているユーザーはどうなりますか?**

「**ユーザー割り当てが必要**」を無効にしても、現在割り当てられているユーザーには影響しません。 このプロパティを無効にすると、すべてのユーザーがアプリケーションにアクセスできるようになるのみです。 リストにあるすべてのユーザーと、アプリケーションのグループに割り当てられているユーザーは引き続き有効です。

- アプリを特定の一連のユーザーに制限する方法については、「- [Azure AD アプリを一連のユーザーに制限する - Microsoft ID プラットフォーム | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.)」を参照してください。
- Azure ポータル内からまたは PowerShell を使用して、Azure Active Directory (Azure AD) のエンタープライズ アプリケーションにユーザーとグループを割り当てる方法については、「[Azure Active Directory でのアプリのユーザー割り当ての管理](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)」を参照してください。
- アプリケーションの作成と管理のアクセス許可を委任するには、「[アプリケーション管理を委任する](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles) - Azure AD | Microsoft Docs」を参照してください。
- **特定のエンタープライズ アプリをユーザーから非表示にする** - 次の手順にしたがって、[**MyApps**] ウィンドウからすべての Microsoft 365 アプリを非表示にします。 アプリは引き続き Office 365 ポータルに表示されます。

 1. ディレクトリのグローバル管理者として Azure ポータルにサインインします。 
 2. [**Azure Active Directory**] を選択します。 
 3. [**ユーザー**] を選択します。 
 4. [**ユーザー設定**] を選択します。 
 5. [**エンタープライズ アプリケーション]** で、[ **エンド ユーザーがアプリケーションを起動して表示する方法を、管理する] をクリックします**。 
 6. ユーザーが **Office 365 ポータルで Office 365 アプリのみしか表示されない** 場合は、[**はい**] をクリックします。 
 7. **[保存]** をクリックします。 
 8. 詳細については、「[Azure AD のユーザーエクスペリエンスからエンタープライズ アプリケーションを非表示にする | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)」を参照してください。

- SaaS (Software as a Service) アプリを多くの組織に提供している場合、任意の Azure Active Directory (Azure AD) テナントからのサインインを承諾するようにアプリを構成することができます。 これは、"アプリケーションをマルチテナントにする" 構成と呼ばれています。 Azure AD テナントのユーザーは、自分のアカウントをアプリで使用することに同意した後、アプリにサインインできます。 詳細については、「[Azure AD ユーザーにサインインするアプリをビルドする - Microsoft ID プラットフォーム | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant)」を参照してください。

- **アプリケーションに割り当てられたエンド ユーザーがアプリケーションにアクセスするには**

エンタープライズ アプリケーション ブレードの各アプリには、エンドユーザーがアクセスするためのリンクがあります。 ユーザーは、**Myapps** ポータルから簡単な方法でアプリにアクセスすることもできます。

- **ユーザーが使用しているアプリケーションおよびアプリケーションの種類を知りたい場合**

**portal.azure.com > Azure Active Directory > サインイン > レポートのダウンロード** から、過去 30 日間のサインインレポートをダウンロードできます。

- [テナント全体の管理者の同意をアプリケーションに付与する](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent)方法と、[エンドユーザーがアプリケーションに同意する方法を構成する](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent)方法について学びます。 

- [同意の機能の仕方](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)を理解し、[アプリケーションへの同意を管理](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests)します。


