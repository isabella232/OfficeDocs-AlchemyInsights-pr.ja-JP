---
title: セキュリティ グループの問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177821"
---
# <a name="issue-with-security-groups"></a>セキュリティ グループの問題

**ネットワーク エラー AADDS104 が発生した場合**

無効なネットワーク セキュリティ グループ ルールは、Azure Active Directory Domain Services (AD DS) のネットワーク エラーの最も一般的な原因です。 仮想ネットワークのネットワーク セキュリティ グループは、特定のポートとプロトコルへのアクセスを許可する必要があります。 これらのポートがブロックされている場合、Azure プラットフォームは管理対象ドメインを監視または更新できません。 Azure AD と Azure AD DS 間の同期も影響を受けます。 サービスの中断を避けるために、既定のポートを開いたままにしてください。

ネットワーク セキュリティ グループの構成の問題に関する一般的なアラートを理解して解決するには、「[セキュリティ グループの追加と確認](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)」を参照してください。
