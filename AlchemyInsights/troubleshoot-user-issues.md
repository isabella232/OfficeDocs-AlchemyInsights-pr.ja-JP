---
title: ユーザーの問題をトラブルシューティングする
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901722"
---
# <a name="announcements"></a>お知らせ

互換性のテストに関する Google のガイダンスに従って、アプリが影響を受けるかどうかをテストします。 Google のガイダンスは https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support で利用できます。

コンシューマー Google アカウントでユーザーにサインインするときは、必ずシステム Web ビューまたはシステム ブラウザーを使用してください。 詳細については、「[Chrome ブラウザのみを使用してアプリケーションにサインインする際の問題](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)」をご覧ください。


**Azure AD ディレクトリに新しいユーザーを作成できません**

Azure AD で新しいユーザーを作成できない問題のトラブルシューティングを行うには、次の手順を実行します。

1. 新しい標準ユーザーを作成する権限があることを確認します。 新しい標準ユーザーを作成できるのは、Azure Active Directory (AD) のグローバル管理者またはユーザー管理者のみです。 これらの役割のいずれにも属していない場合は、管理者にこれらの役割のいずれかに追加してもらうか、新しいユーザー アカウントを作成するように依頼してください。
2. ユーザー名が Azure AD で確認済みのドメインにあることを確認してください。 Azure AD に確認済みのカスタム ドメイン名がない場合は、*.onmicrosoft.com で終わる Azure AD イニシャル ドメインを使用できます。
3. ユーザー名が、オンプレミス AD から Azure AD にフェデレーションされていないドメインにあることを確認してください。 オンプレミスからフェデレーションされたドメイン名でユーザーをクラウドに追加することはできません。
4. 新しいユーザーに割り当てるユーザー名が、他のユーザーまたは連絡先にないことを確認してください。 ユーザー名は、Azure AD 全体で一意である必要があります。
5. 「[Azure Active Directory でのロールと管理者](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators)」を参照してください。
6. Azure AD の[ドメイン名](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains)を確認してください。
7. [監査ログ](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit)を確認して、アクションを実行したユーザーとタイミングなど、最近作成または削除されたユーザーに関する詳細情報を確認します。
8. 新しいユーザーの追加の詳細については、「[Azure portal を使用して Azure AD に新しいユーザーを作成する](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)」を参照してください。
9. Azure AD の管理者ロールのアクセス許可の詳細については、「[Azure AD の管理者ロール](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)」を参照してください。
10. Azure AD Powershell を使用してユーザーを作成する方法の詳細については、「[Azure AD PowerShell を使用して新しいユーザーを作成する](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser)」を参照してください。

**セルフサービスのサインアップでの問題**

セルフサービス サインアップに関する問題のトラブルシューティングを行うには、次の手順を実行します。

1. アプリケーションでセルフサービス サインアップを使用するには、まずテナントのセルフサービス サインアップを有効にします。 
2. アプリケーションがセルフサービス サインアップをサポートできるようにするには、アプリケーションをユーザーフローに追加します。 次回そのアプリケーションのログイン ページにアクセスすると、**_アカウントをお持ちではありませんか? アカウントを作成_* _ というオプションが表示されます。 これにより、セルフサービスのサインアップ プロセスが開始されます。
3. セルフサービス サインアップを使用して Azure AD の組織にデータを入力する方法については、「[Azure ADのセルフサービス サインアップ](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup)」を参照してください。
4. ユーザーフローを 1 つ以上のアプリケーションに関連付けると、そのアプリにアクセスするユーザーは、ユーザー フローで構成されたオプションを使用して、サインアップしてゲスト アカウントを取得できるようになります。 サインアップとゲスト アカウントの取得の詳細については、ユーザーは「[ゲストユーザーのセルフサービス サインアップ](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow)」を参照してください。

_ *外部ユーザーの招待に関する問題**

外部ユーザーの招待に関する問題のトラブルシューティングを行うには、次の手順を実行します。

ユーザーがサインインする名前と一致するメール アドレスにユーザーの招待を送信するようにしてください。 ユーザーのプロキシ メール アドレスに招待状を送信した場合、ユーザーは有効にすることができません。 詳細については、「[Azure AD B2B ドキュメント](https://docs.microsoft.com/azure/active-directory/external-identities/)」を参照してください。

**ユーザーにライセンスを割り当てることができません**

ライセンスの割り当てに関する問題のトラブルシューティングを行うには、次の手順を実行します。

1. ユーザー ライセンスを管理するには、グローバル管理者、ライセンス管理者、またはユーザー管理者のいずれかの必要な管理者ロールを持つアカウントを使用していることを確認してください。 ユーザーの役割は、ユーザー ブレードの **[ディレクトリの役割]** タブで確認できます。
2. Azure ポータルを使用していて、ライセンスの割り当てが失敗する場合は、右上隅にある通知をクリックします。 これにより、どこに問題があったのかについての詳細が記載されたブレードが開きます。 ほとんどの場合、それで問題を理解して解決することができます。
3. ライセンスをユーザーに割り当てる前に、**Usage Location** プロパティがユーザーに設定されていることを確認してください。 ユーザー ブレードの **[プロファイル]** タブを表示して、ユーザーがそのプロパティを設定していることを確認します。
4. 割り当てようとしている製品に、使用可能なライセンスが十分にあることを確認してください。 使用可能なライセンスの数は、Azure ポータルの [[Azure Active Directory] -> [ライセンス] -> [すべての製品]](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products) で確認できます。
5. ユーザーは、割り当てようとしている新しいライセンスのサービスと競合するサービスを持つ別のライセンスをすでに持っている可能性があります。 たとえば、ユーザーが Exchange Online (プラン 1) サービスを有効にしている場合、Exchange Online (プラン 2) でライセンスを割り当てることはできません。 サービスの 1 つを無効にして、新しいライセンスの割り当てを許可します。 Azure ポータルまたは PowerShell コマンドレットを使用している場合、**問題の詳細** ページには、競合の原因となっている特定のサービスが一覧表示されます。
6. ライセンスを削除しようとして失敗した場合、ユーザーは、削除しようとしているサービスに依存するサービスを持つ他のライセンスを持っている可能性があります。 Azure ポータルまたは PowerShell コマンドレットを使用している場合、エラーメッセージには、依存関係がある特定のサービスが一覧表示されます。
7. ライセンスがユーザーから追加/削除された理由 (たとえば、組織内の他のユーザーが変更を加えた可能性がある) を理解したい場合は、監査ログを確認してください。 フィルタを **ライセンス アクティビティ** に設定して、それらを実行した "アクター" を含むすべての変更を表示します。
8. Exchange Online を使用している場合、テナント内の一部のユーザーが同じプロキシ アドレス値で誤って構成されている可能性があります。 このような場合、ライセンス操作が失敗すると、一般的なエラー メッセージが表示されることがあります。 [この記事](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used)には、[リモート PowerShell を使用して Exchange Online に接続する方法](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)など、この問題に関する詳細情報が含まれています。テナント内のどのユーザーに同じプロキシ アドレスが含まれているかを特定するには、次の Exchange Online コマンドレットを実行します。

実行

Get-Recipient | where {$_.EmailAddresses -match <user principal name>} | fL Name, RecipientType,emailaddresses





