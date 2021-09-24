---
title: サブドメインの追加
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506147"
---
# <a name="adding-a-sub-domain"></a>サブドメインの追加

サブドメインは、親ドメインと同じテナントまたは別のテナントに追加できます。 いずれの場合にも、レジストラーの Web サイトで DNS 設定を自分で管理する必要があります。 Microsoft が NS レコードを使用して DNS 設定を管理できるようにする場合、または Microsoft からドメインを購入した場合は、最初にこれを変更しないとサブドメインを追加できません。

最初に親ドメインを追加してから、サブドメインを追加します。 サブドメインが同じテナントにある場合は、追加の検証は必要ありません。 別のテナントにサブドメインを追加する場合、選択したサービスのドメインと追加の DNS レコードを追加する前に、所有権の検証に DNS txt レコードが必要です。

- ドメインまたはサブドメインを追加するには、[[ドメインの追加ウィザード]](https://admin.microsoft.com/Adminportal#/Domains/Wizard) に従います。または、ドメインまたはサブドメインを手動で追加するには **[設定]**  >  **[ドメイン]**  >  **[ドメインの追加]** の順に進みます。

必要に応じて、次の手順を実行します:

- 既存のドメインの DNS 設定を管理するユーザーを変更するには、**[設定]**  > [ **[ドメイン]**](https://admin.microsoft.com/Adminportal/Home#/Domains)に移動し、ドメインの横にあるチェック ボックスをオンにして **[DNSの管理]** を選択します。 ウィザードで **[独自の DNS レコードを追加]** を選択し、ウィザードを完了します。
- Microsoft から購入したドメインにサブドメインを追加するには、まずドメインを別のレジストラーに転送してから、上記の変更を行って独自の DNS レコードを管理します。 詳細については、「[Microsoft から別のホストにドメインを移行する](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)」を参照してください。
- ドメインが組織内の他のメンバーまたはユーザーによって既に使用されているというエラーが表示された場合は、ドメインを使用する前に、まずこの管理されていないアカウントを引き継ぐ必要があります。 手順については、「[管理されていないディレクトリを Azure Active Directory の管理者として引き継ぐ](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover)」を参照してください。
