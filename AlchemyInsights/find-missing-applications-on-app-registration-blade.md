---
title: アプリ登録ブレードで不足しているアプリケーションを見つける
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9654"
ms.openlocfilehash: 0dee7e44a8701e1df924b9657cce6cf9d90160e58277d667f6069a4cbcf87ce5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057107"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>アプリ登録ブレードで不足しているアプリケーションを見つける

1. アプリ登録ポータルでアプリケーションが見つかりません。

    アプリケーションがマルチテナント アプリケーションであり、別のテナントに登録されている場合、そのアプリケーションは [アプリ登録] ブレードに表示されません。 ただし、 (同意された後) アクセスされ、テナントでサービス プリンシパルが作成されると、[エンタープライズ アプリケーション] ブレードの下に表示される場合があります。 詳細については、「[Azure ADのアプリとサービス プリンシパル-Microsoft ID プラットフォーム](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)」を参照してください。
2. 管理者であるにもかかわらず、アプリ登録ブレードでアプリを表示できません。

    Azure ポータルの正しいディレクトリにいることを確認してください。
3. マイ アプリケーションは [エンタープライズ アプリケーション] ブレードに表示されませんが、PowerShell コマンドをクエリすると表示されます。

    Azure ポータルからアプリケーションを削除した後、ポータルに表示されない場合がありますが、完全に削除されていない可能性があります。 詳細については、以下を参照してください。
    - Powershell コマンド **Get-AzureADDeletedApplication** を使用して、以前に削除されたアプリケーションのリストを取得し、アプリケーションがリストに表示されるかどうかを確認できます。 詳細については、[Get-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication) を参照してください。
    - アプリケーションを完全に削除する場合は、PowerShellで次のコマンドを試すことができます: **Remove-AzureADApplication -ObjectId**。 詳細については、[Remove-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication) を参照してください。
    - または、次の Powershell コマンドを使用して、削除されたアプリケーションの復元を試すことができます: **Restore AzureADDeletedApplication -ObjectId**。 詳細については、[Restore-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication) を参照してください。
4. 新しい Azure テナントにプリインストールされているすべてのエンタープライズ アプリケーションのリストが見つかりません。

    既定では、AzureAD にはプリインストールされたエンタープライズ アプリケーションはありません。 Azure AD ギャラリーから参照して [新しいアプリケーション] オプションから手動で追加するか、ギャラリー以外のアプリケーションを追加する必要があります。 詳細については、「[クイックスタート: Azure Active Directory (Azure AD) テナントにアプリケーションを追加する](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)」を参照してください。
    グローバル管理者の場合は、[Microsoft 365 App Launcher](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher) を使用してアプリに簡単にアクセスできます。
5. マイ アプリ ポータルからアプリが見つかりません。

    アプリが [マイ アプリ] コレクション ページで非表示になっていないことを確認してください。 詳細については、[マイ アプリ ポータル - Azure AD のコレクション (プレビュー)](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections) を参照してください。
6. My Apps ポータルからアプリを起動するには、「[マイ アプリ ポータルでアプリを見つけて使用する - AzureAD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)」を参照してください。
7. インストール後、Office 365 Mover アプリがエンタープライズ アプリケーション ブレードに表示されません。

    「Office 365 Mover」アプリケーションはマルチ テナント アプリであり、エンタープライズ アプリ登録の [ギャラリー アプリケーション] セクションを使用して AAD に追加する必要はありません。 Office 365 Mover アプリにアクセスするには、アプリにサインインするだけで、アクセス許可についてユーザーの同意を求められます。 ユーザーが同意を提供すると、このアプリは、ログインしたメール ID でテナントに自動的に追加されます。

    アプリケーションにサインインすると、AAD のエンタープライズ アプリケーションのブレードの下にこのアプリケーションのエントリが表示されるはずです。 フルネーム ("Office 365 Mover" など) 入力するか、単に「office」を検索してそのアプリケーションを検索する必要があります。そうすると、アプリが一覧表示されます。 詳細については、「[Office 365 Mover がインストール済みとありますが、エンタープライズ アプリケーション ギャラリーに表示されていません](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)」をご覧ください。
8. 「[クイック スタート: Azure Active Directory (Azure AD) テナントを ID 管理用に使用しているアプリケーションの一覧を表示する](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal)」で、Azure AD テナントを ID プロバイダー (IdP) として使用するように既にセットアップされているアプリケーション (アプリとも呼ばれる) を表示する方法を説明します。
9. [Azure Active Directory へのアプリケーションの追加または削除に関する一般的な問題のトラブルシューティング](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps)は、Azure Active Directory でアプリを表示するときに発生する一般的な問題を理解するのに役立ちます。
