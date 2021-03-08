---
title: AD ユーザー プロビジョニングへの稼働日が隔離状態になります
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/04/2021
ms.locfileid: "50484063"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>AD ユーザー プロビジョニングへの稼働日が隔離状態になります

**AD ユーザー プロビジョニングへの稼働日が隔離状態になり、AD でユーザーが作成されません**

AD ユーザー プロビジョニングへの稼働日ジョブが隔離状態になり、監査ログにエクスポートの失敗イベントが表示され、エラーメッセージ **Error: OperationsError-SvcErr: Operationerror が発生しました。 ディレクトリ サービスの上位参照は設定されていません。 したがって、ディレクトリ サービスは、このフォレスト外のオブジェクトへの参照を発行できません**。 このエラーは通常、Active Directory コンテナ OU が正しく設定されていない場合、または **parentDistinguishedName** に使用される式マッピングに問題がある場合に表示されます。

タイプミスについては、「**新規ユーザー** のデフォルト OU」パラメーターを確認してください。 指定された OU が AD にすでに存在することを確認してください。 属性マッピングで **parentDistinguishedName** を使用している場合は、AD ドメイン内の既知のコンテナーに対して常に評価されることを確認してください。 生成された値を確認するには、監査ログの Export イベントを確認してください。

自動プロビジョニング用の Workday の構成の詳細については、「[チュートリアル: Workday を構成し、自動ユーザー プロビジョニングに対応させる](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)」を参照してください。

