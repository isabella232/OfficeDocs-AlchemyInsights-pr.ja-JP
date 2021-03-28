---
title: Yammer 管理者について
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
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/22/2021
ms.locfileid: "51038355"
---
# <a name="about-yammer-admins"></a>Yammer 管理者について

**ネットワーク管理者**

グローバル管理者は Yammer ネットワークの認証管理者の役割に自動的に昇格します。 次の場合、この昇格が正しく行われません。

- 複数の Yammer ネットワークが存在し、管理者が間違ったネットワークにサインインしている。 1 つの Yammer ネットワークに到達するには、[ネットワークの統合](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)が必要です。
- Azure PIM が使用されています。 ユーザーがグローバル管理者に昇格するまでに、長く時間が必要な場合があります。 Yammer の今後の更新でこの問題が解決される場合がありますが、ユーザーのグローバル管理者への昇格は手動で行うのが最善です。
- Yammer ネットワークに同期の問題があります。 この場合、さらに調査するためにはサポートの依頼が必要になります。

Yammer 管理者の役割の詳細については、「[Yammer の管理者の役割を管理する](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins)」を参照してください。

**グループ管理者**

Microsoft 365 に接続されているグループのグループ管理者は、Azure AD のグループ メンバーシップと同期されます。 大規模なグループの場合、この同期が長期間におよぶ場合があります。
