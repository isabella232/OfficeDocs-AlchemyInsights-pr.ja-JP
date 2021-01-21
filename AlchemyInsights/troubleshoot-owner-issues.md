---
title: 所有者の問題のトラブルシューティング
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7815"
- "9004358"
ms.openlocfilehash: 914d5682a403197a8569bb75fda8a77449f485f6
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901717"
---
# <a name="troubleshoot-owner-issues"></a>所有者の問題のトラブルシューティング

所有者関連の問題のトラブルシューティングを行うには、次の手順を実行します。

1. [Azure サブスクリプション管理者を追加または変更する](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure Active Directory (Azure AD) グループは、グループ所有者によって所有および管理されます。 グループ所有者は、ユーザーまたはサービス プリンシパルであり、メンバーシップを含めたグループを管理できます。 グループ所有者を割り当てることができるのは、既存のグループ所有者またはグループを管理する管理者のみです。 グループ所有者がグループのメンバーである必要はありません。
2. [[Azure サブスクリプション管理者の追加または変更]](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): この記事では、サブスクリプションの範囲で Azure RBAC を使用するユーザーの管理者役割を追加または変更する方法について説明します。
3. PowerShell を使用して、グループ所有者またはアプリケーション所有者を追加します。
