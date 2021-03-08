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
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="ba749-102">AD ユーザー プロビジョニングへの稼働日が隔離状態になります</span><span class="sxs-lookup"><span data-stu-id="ba749-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="ba749-103">**AD ユーザー プロビジョニングへの稼働日が隔離状態になり、AD でユーザーが作成されません**</span><span class="sxs-lookup"><span data-stu-id="ba749-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="ba749-104">AD ユーザー プロビジョニングへの稼働日ジョブが隔離状態になり、監査ログにエクスポートの失敗イベントが表示され、エラーメッセージ **Error: OperationsError-SvcErr: Operationerror が発生しました。 ディレクトリ サービスの上位参照は設定されていません。 したがって、ディレクトリ サービスは、このフォレスト外のオブジェクトへの参照を発行できません**。</span><span class="sxs-lookup"><span data-stu-id="ba749-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="ba749-105">このエラーは通常、Active Directory コンテナ OU が正しく設定されていない場合、または **parentDistinguishedName** に使用される式マッピングに問題がある場合に表示されます。</span><span class="sxs-lookup"><span data-stu-id="ba749-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="ba749-106">タイプミスについては、「**新規ユーザー** のデフォルト OU」パラメーターを確認してください。</span><span class="sxs-lookup"><span data-stu-id="ba749-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="ba749-107">指定された OU が AD にすでに存在することを確認してください。</span><span class="sxs-lookup"><span data-stu-id="ba749-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="ba749-108">属性マッピングで **parentDistinguishedName** を使用している場合は、AD ドメイン内の既知のコンテナーに対して常に評価されることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="ba749-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="ba749-109">生成された値を確認するには、監査ログの Export イベントを確認してください。</span><span class="sxs-lookup"><span data-stu-id="ba749-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="ba749-110">自動プロビジョニング用の Workday の構成の詳細については、「[チュートリアル: Workday を構成し、自動ユーザー プロビジョニングに対応させる](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ba749-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

