---
title: user の作成
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 800baae2d748708d8cb7a5fb0e73fce5dcf455cb
ms.sourcegitcommit: 2d617ae59eed0ce8b571339ceefce6473c03b94c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "52569736"
---
# <a name="create-user"></a>ユーザーを作成する

**お知らせ:**

- [2021 年 1 月 4 日以降、Google は WebView サインインのサポートを廃止します](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support)。 互換性のテストに関する [Google のガイダンス](https://go.microsoft.com/fwlink/?linkid=2157323)に従って、アプリが影響を受けるかどうかをテストします。
- コンシューマー向けの Google アカウントでユーザーにサインインするときは、必ずシステム WebView またはシステム ブラウザーを使用してください。 詳細については、「[Chrome ブラウザのみを使用してアプリケーションにサインインする際の問題](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)」をご覧ください。

**Azure AD ディレクトリに新しいユーザーを作成できません**

1. 新しい標準ユーザーを作成する権限があることを確認します。 新しい標準ユーザーを作成できるのは、Azure Active Directory (AD) のグローバル管理者またはユーザー管理者のみです。 これらの役割のいずれにも属していない場合は、管理者にこれらの役割のいずれかに追加してもらうか、新しいユーザー アカウントを作成するように依頼してください。
1. ユーザー名が Azure AD で確認済みのドメインにあることを確認してください。 Azure AD に確認済みのカスタム ドメイン名がない場合は、*.onmicrosoft.com で終わる Azure AD イニシャル ドメインを使用できます。
1. ユーザー名が、オンプレミス AD から Azure AD にフェデレーションされていないドメインにあることを確認してください。 オンプレミスからフェデレーションされたドメイン名でユーザーをクラウドに追加することはできません。
1. 新しいユーザーに割り当てるユーザー名が、他のユーザーまたは連絡先にないことを確認してください。 ユーザー名は、Azure AD 全体で一意である必要があります。
1. 「[Azure Active Directory でのロールと管理者](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators)」を参照してください。
1. Azure AD の[ドメイン名](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators)を確認してください。
1. [監査ログ](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators)を確認して、アクションを実行したユーザーとタイミングなど、最近作成または削除されたユーザーに関する詳細情報を確認します。
1. 新しいユーザーの追加の詳細については、「[Azure portal を使用して Azure AD に新しいユーザーを作成する](/azure/active-directory/active-directory-users-create-azure-portal)」を参照してください。
1. [Azure AD での管理者の役割](/azure/active-directory/active-directory-assign-admin-roles): Azure Active Directory での管理者の役割のアクセス許可
1. [Azure AD PowerShell を使用して新しいユーザーを作成する](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)こともできます。
