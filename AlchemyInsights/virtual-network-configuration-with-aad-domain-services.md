---
title: AAD Domain Services を使用した仮想構成
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
- "7927"
- "9004397"
ms.openlocfilehash: 03a6ec63ba8e2779b0fe3f0381606af2c0748f8b848baaa7cd88b61317bd7a5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072849"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>AAD Domain Services を使用した仮想構成

AAD Domain Services を使用した仮想構成には、次の手順が含まれます。 

1. Azure portal https://aka.ms/aadds-health でドメインの正常性を確認する
2. ポータル https://aka.ms/aadds-networking の Azure AD Domain Services で同期するために必要なポートをブロックするルールがないか NSG を確認する
3. 仮想ネットワークが Azure AD Domain Services の管理ドメインと同じ Azure リージョンに展開されていることを確認します。
4. 仮想ネットワークで使用可能なドメイン名が同じである既存のドメインがないことを確認します。

AAD Domain Services をサポートする Azure 仮想ネットワークの設計上の考慮事項の詳細については、「[仮想ネットワークの考慮事項](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations)」を参照してください。

