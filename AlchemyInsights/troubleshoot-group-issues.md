---
title: グループの問題のトラブルシューティング
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
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886943"
---
# <a name="troubleshoot-group-issues"></a>グループの問題のトラブルシューティング

**Azure AD 役割にグループを割り当てる必要がある**

Azure Active Directory (AD) グループを Azure AD 役割に割り当てるには、次の手順を実行します。

1. [新しいグループを作成する] - 新しいグループを作成するには、次の手順を実行します。

    a. 特権役割の管理者または全体管理者の権限を持つ Azure AD 管理センターにサインインします。 
    b. [Azure Active Directory]、[グループ]、[すべてのグループ]、[新しいグループ] の順に選択します。 
    c. グループを作成します。

2. グループの作成中またはグループの作成後に、役割をグループに割り当てます。

    a. グループの作成時にグループに役割を割り当てるには、[Azure AD 役割をグループに割り当てることができます] トグルをオンにし、グループを作成します。
    b. 作成後にグループに役割を割り当てるには、新しく作成したグループの [割り当てられている役割] タブに移動し、その役割をグループに割り当てます。

**Azure AD 役割に割り当てられたグループのメンバシップを管理する必要がある**

1. 特権を昇格させないために、既定では、特権役割の管理者と全体管理者だけが、役割に割り当てられているグループのメンバシップを変更できます。 ただし、このようなグループに所有者を割り当て、このタスクを委任することもできます。 詳細については、「[クラウド グループを使用して、Azure Active Directory の役割の割り当てを管理する](https://docs.microsoft.com/azure/active-directory/roles/groups-concept)」を参照してください。
2. Azure AD のグループに役割を割り当てる際の一般的な質問とトラブルシューティングのヒントについては、「[クラウド グループに割り当てられた役割のトラブルシューティング](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)」を参照してください。

**動的グループ**

1. 組み込みのユーザーの属性が見つからない場合は、その属性がサポートされているプロパティのリストにあることを確認します。
2. 組み込みのデバイスの属性を検索する場合は、属性がデバイスの属性のリストにあることを確認します。 
3. 組み込みのユーザーの属性およびデバイスの属性に加えて、[拡張属性](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties)も使用できます。 オンプレミス Windows Server AD または接続された SaaS アプリケーションから拡張属性を同期すると、規則ビルダーのドロップダウン リストに属性が表示されます。 カスタム属性名は、PowerShell を使用してユーザーの属性を照会し、属性名を検索することにより、ディレクトリ内で見つけることができます。 これらは、規則構文で規則を作成する場合にも使用できます。
4. テナントが適切なライセンスを持っていることを確認します。 動的グループでは、テナントに Azure AD P1 Premium ライセンスが必要です。 Azure AD ライセンス プランのリストは、[こちら](https://azure.microsoft.com/pricing/details/active-directory/)でアクセスできます。 Enterprise Mobility + Security ライセンス プランは、[こちら](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing)でアクセスできます。
5. 動的グループを作成するユーザーの役割が、全体管理者、Intune 管理者、グループ管理者、またはユーザー管理者であることを確認します。
6. グループが入力されるまでしばらくお待ちください。 テナントのサイズによっては、最初または規則変更後にグループを入力するのに最大 24 時間かかる場合があります。
7. 詳細については、「[動的グループ メンバシップ用の属性ベースの規則の作成](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership)」を参照してください。

**グループを削除する必要がある**

1. グループは、Azure AD Powershell モジュールの Remove-AzureADGroup コマンドレットを使用してディレクトリから削除できます。
2. Azure AD で同期グループを削除する前に、エラーを回避するために割り当てられたライセンスがすべて削除されていることを確認します。
3. グループの削除の詳細については、「[ライセンスが割り当てられているグループの削除](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license)」を参照してください。

**削除したグループを復元する必要がある**

1. Office 365 グループが削除された場合、完全な削除が行われる 30 日前までしか復元できません。 完全に削除されると、グループは復元できなくなります。 グループの復元の詳細は、[こちら](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)を参照してください。
2. この機能は、セキュリティ グループおよび配布グループではサポートされません。
3. Office 365 グループの復元が承認されていることを確認します。 全体管理者、グループ管理者、ユーザー アカウント管理者、Intune サービス管理者、パートナー レベル 1 または レベル 2 のサポート、およびグループ所有者はグループを復元できます。
4. 動的グループを削除して復元すると、そのグループは新しいグループと見なされ、規則に従って再入力されます。 このプロセスには最大 24 時間かかる場合があります。
5. 削除されたグループの復元の詳細については、「[Azure Active Directory で削除された Office 365 グループを復元する](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)」を参照してください。

**グループの有効期限ポリシーの構成**

1. この機能は Office 365 グループのみでサポートされ、セキュリティ グループおよび配布グループではサポートされません。
2. Office 365 グループの有効期限ポリシーを構成および使用するには、Azure AD Premium ライセンスが必要です。
3. 現在、テナント上の Office 365 グループに構成できる有効期限ポリシーは 1 つのみです。
4. グループを更新できるのは、全体管理者、グループ管理者、ユーザー管理者、およびグループ所有者だけです。
5. Office 365 グループの有効期限が切れると、そのグループは削除され、完全な削除が行われる 30 日前までしか復元できません。 完全に削除されると、グループは復元できなくなります。 グループの復元の詳細は、[こちら](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)を参照してください。

**アクティビティ ベースの自動更新**

SharePoint、Outlook、および Teams のユーザー アクティビティによって、グループの自動更新がトリガーされます。 アクティビティは、グループが期限切れになる 35 日前に確認されます。 現在のグループの有効期限中にアクティビティが発生した場合、グループは自動的に更新され、メール通知はグループ所有者に送信されません。

**期限切れグループの通知タイミング**

1. メール通知は、グループの有効期限の 30 日前、15 日前、および 1 日前に Office 365 グループ所有者に送信されます。
2. 最初に有効期限を設定したとき、有効期限の間隔より古いグループは、有効期限まで 35 日に設定されます。
3. グループの有効期限は、ポリシーの更新日ではなく、グループの更新日に基づいて計算されます。 有効期限ポリシーが更新されても、有効期限は変更されません。
4. 詳細については、「[グループの有効期限ポリシーと更新メール](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle)」および「[削除した Office 365 グループを Azure Active Directory に復元する](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)」を参照してください。

**グループを作成する権限**

新しいグループを作成する権限があることを確認します。 グローバル管理者は、Azure ポータルまたはアクセス パネルでグループの作成を無効にできます。 新しいグループを作成したり、適切な権限を付与したりするには、管理者が必要になる場合があります。

1. [Azure portal で新しいグループを作成し、メンバを追加する](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [Powershell MS Online でグループを作成する](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [Powershell でグループの作成を無効にする](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [Office 365 でグループを作成できるユーザーを管理する](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [Powershell を介した Office 365 ウェルカム通知を無効にする](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Azure AD 管理者の役割](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**グループ作成権限を管理する**

1. 全体管理者は、**[すべてのグループ]、[全般 (設定)]** の順に移動し、**[ユーザーは Azure portal でセキュリティ グループを作成できます]** または **[ユーザーは Azure portal で Office 365 グループを作成できます]** を設定することにより、セキュリティ上の理由でグループ作成のアクセス許可、Azure portal、またはアクセス パネルで作成された Office 365 グループを管理できます。
2. Azure AD P1 Premium ライセンスをお持ちの場合は、グループの作成を制限してユーザーのグループを選択することもできます。

**新しい Office 365 グループ メンバーのウェルカム通知を無効にする**

Office 365 グループに追加されたユーザーに送信されるウェルカム通知を無効にするには、Powershell で `UnifiedGroupWelcomeMessageEnabled` を **False** に設定します。 この設定については、[こちら](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)をご覧ください。













