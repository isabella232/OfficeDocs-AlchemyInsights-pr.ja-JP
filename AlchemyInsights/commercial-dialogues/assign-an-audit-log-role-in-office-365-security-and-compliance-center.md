---
title: Office 365 セキュリティ/コンプライアンス センターで監査ログの役割を割り当てる
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751334"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a>Office 365 セキュリティ/コンプライアンス センターで監査ログの役割を割り当てる

Office 365 の監査ログを検索するには、管理者には Exchange Online で **閲覧限定の監査ログ** の役割または **監査ログ** の役割が割り当てられている必要があります。 既定では、これらの役割はコンプライアンス管理役割グループまたは組織管理役割グループに割り当てられています。 Office 365 および Microsoft 365 のグローバル管理者は自動的に、組織管理役割グループのメンバーとして追加されます。

ユーザーが最小限の特権レベルで検索できるようにするには、Exchange Online でカスタムの役割グループを作成し、**閲覧限定の監査ログ** の役割または **監査ログ** の役割を追加し、この新しい役割グループのメンバーとしてユーザーを追加します。

詳細については、「[Exchange Online で役割グループを管理する](https://docs.microsoft.com/Exchange/permissions-exo/role-groups)」および「[セキュリティ/コンプライアンス センターで監査ログを検索する](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)」を参照してください。