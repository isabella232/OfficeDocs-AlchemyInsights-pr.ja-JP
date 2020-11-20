---
title: 特権 ID 管理のロール
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089264"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="74976-102">特権 ID 管理 (PIM) のロール</span><span class="sxs-lookup"><span data-stu-id="74976-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="74976-103">**ロールのアクティブ化を行った後、権限が付与されない**</span><span class="sxs-lookup"><span data-stu-id="74976-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="74976-104">Azure AD Privileged Identity Management（PIM）でロールをアクティブ化すると、そのアクティブ化が、特権ロールを必要とするすべてのポータルに即座に伝達されない場合があります。</span><span class="sxs-lookup"><span data-stu-id="74976-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="74976-105">場合によっては、変更が伝播されたとしても、ポータルで Web キャッシュを行うと、変更がすぐに有効にならないことがあります。</span><span class="sxs-lookup"><span data-stu-id="74976-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="74976-106">アクティブ化が遅れる場合は、次の手順に従ってください。</span><span class="sxs-lookup"><span data-stu-id="74976-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="74976-107">Azure ポータルからサインアウトしてから、再度サインインします。</span><span class="sxs-lookup"><span data-stu-id="74976-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="74976-108">Azure AD ロールまたは Azure リソース ロールをアクティブ化すると、アクティブ化のステージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="74976-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="74976-109">すべての段階が完了すると、「サインアウト」リンクが表示されます。</span><span class="sxs-lookup"><span data-stu-id="74976-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="74976-110">このリンクを使用してサインアウトできます。 これにより、アクティブ化遅延のほとんどの場合が解決されます。</span><span class="sxs-lookup"><span data-stu-id="74976-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="74976-111">PIMで、自分がロールのメンバーとしてリストされていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="74976-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="74976-112">Exchange 管理者ロールをアクティブ化する場合は、必ずサインアウトしてから再度サインインしてください。</span><span class="sxs-lookup"><span data-stu-id="74976-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="74976-113">問題が解決しない場合は、サポート チケットを開き、問題として提起します。</span><span class="sxs-lookup"><span data-stu-id="74976-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="74976-114">Exchange 管理者ロールを使用してセキュリティ/コンプライアンス センターにアクセスしている場合は、次の手順を参照してください。</span><span class="sxs-lookup"><span data-stu-id="74976-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="74976-115">セキュリティ/コンプライアンス センターにアクセスするためにロールをアクティブ化する場合、または SharePoint 管理者のロールをアクティブ化する場合、数分から数時間までのアクティブ化の遅延が発生します。</span><span class="sxs-lookup"><span data-stu-id="74976-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="74976-116">これは既知の問題であり、これらのチームと積極的に協力して、この問題をできるだけ早く解決できるよう取り組んでいます。</span><span class="sxs-lookup"><span data-stu-id="74976-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="74976-117">詳しくは、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="74976-117">For more information, see:</span></span>

- [<span data-ttu-id="74976-118">PIM で Azure AD ロールをアクティブ化する</span><span class="sxs-lookup"><span data-stu-id="74976-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="74976-119">PIM で Azure リソース ロールをアクティブ化する</span><span class="sxs-lookup"><span data-stu-id="74976-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="74976-120">**ロールを非アクティブ化した後、またはロールのアクティブ化の有効期限が切れた後、アクセス許可が削除されない**</span><span class="sxs-lookup"><span data-stu-id="74976-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="74976-121">Azure AD Privileged Identity Management でロールを非アクティブ化する場合、またはロールのアクティブ化期間が終了すると、引き続きアクセスできるようになるまでに遅延が発生する場合があります。</span><span class="sxs-lookup"><span data-stu-id="74976-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="74976-122">非アクティブ化が遅れる場合は、次の手順に従ってください。</span><span class="sxs-lookup"><span data-stu-id="74976-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="74976-123">Exchange管理者ロールを非アクティブ化する場合、またはロールのアクティブ化期間が満了していて、権限が削除されるまでに大幅な遅延が発生していることに気づいた場合は、サポート チケットを開き、サポート エンジニアに、この問題について Office 内の特権アクセス管理 (PAM) チームにチケットを提出するのを手伝ってもらうように伝えます。</span><span class="sxs-lookup"><span data-stu-id="74976-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="74976-124">アクティベーション期間が終了してもブラウザー セッションが開いている場合は、ブラウザーを閉じてください。</span><span class="sxs-lookup"><span data-stu-id="74976-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="74976-125">そのセッションを閉じるまで、ロールを引き続き使用できます。</span><span class="sxs-lookup"><span data-stu-id="74976-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="74976-126">これは既知の問題であり、アクティベーションの有効期限が切れたときに、各セッションをアクティブに取り消すための修正の可能性を検討しています。</span><span class="sxs-lookup"><span data-stu-id="74976-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="74976-127">この2つのシナリオとは異なる遅延がある場合は、サポート チケットを開いてください。</span><span class="sxs-lookup"><span data-stu-id="74976-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
