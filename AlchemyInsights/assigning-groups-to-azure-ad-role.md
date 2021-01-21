---
title: Azure AD 役割へのグループの割り当て
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
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885801"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Azure AD 役割へのグループの割り当て

Azure AD の権限ソースを持つ Azure AD グループを Azure AD 役割に割り当てるには、次の手順を実行します。

1. [新しいグループを作成する] - 新しいグループを作成するには、次の手順を実行します。

    a. **特権役割の管理者** または **全体管理者** の権限を持つ Azure AD 管理センターにサインインします。
    b. **[Azure Active Directory]、[グループ]、[すべてのグループ]、[新しいグループ]** の順に選択します。
    c. グループを作成します。

2. グループの作成中またはグループの作成後に、役割をグループに割り当てます。

    a. グループの作成時にグループに役割を割り当てるには、**[Azure AD 役割をグループに割り当てることができます]** トグルをオンにし、グループを作成します。
    b. 作成後にグループに役割を割り当てるには、新しく作成したグループの **[割り当てられている役割]** タブに移動し、その役割をグループに割り当てます。  

**Azure AD 役割に割り当てられたグループのメンバシップを管理する**

特権を昇格させないために、既定では、特権役割の管理者と全体管理者だけが、役割に割り当てられているグループのメンバシップを変更できます。 ただし、このようなグループに所有者を割り当て、このタスクを委任することもできます。

クラウド グループを Azure AD 役割に割り当てる方法の詳細については、「[クラウド グループに AD 役割を割り当てる](https://docs.microsoft.com/azure/active-directory/roles/groups-concept)」を参照してください。 クラウド グループに割り当てられたトラブルシューティングの役割の詳細については、「[クラウド グループに割り当てられた役割のトラブルシューティング](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)」を参照してください。





