---
title: グループ同期
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 7e5ed69c34f8e7b922d7eef202af508152a7e04d7773581b32e43395571c6fbc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53987652"
---
# <a name="group-sync"></a>グループ同期

この記事では、グループ同期に関するガイダンスを提供します。

1. グローバル管理者またはグループ所有者が Azure portal でグループのプロパティを変更したり、メンバーを追加したり、所有者を割り当てたりできない場合は、グループの権限ソースが、グローバル管理者またはグループ所有者がグループを変更するための Azure Active Directory (Azure AD) であることを確認してください。
2. Azure AD で同期済みのグループを削除する前に、エラーを回避するために[割り当てられたライセンスがすべて削除されている](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced)ことを確認します。

ユーザー、グループ、連絡先を同期する方法については、「[Azure AD Connect 同期](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)」を参照してください。AD Connect を使用してオンプレミス グループを同期するには、「[Azure AD Connect を使用したオンプレミス グループの Azure への同期](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support)」に従ってください。

同期中の一般的なエラーのトラブルシューティングを行うには、こちらのガイド「[同期中のエラーのトラブルシューティング](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors)」に従ってください。

