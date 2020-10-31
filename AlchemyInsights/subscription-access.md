---
title: サブスクリプションへのアクセス
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/27/2020
ms.locfileid: "48808197"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="f242a-102">ブラウザーの問題が原因で、Azure にサインインできない (ブラウザーがハングする、処理中のままである、読み込みできないなど)</span><span class="sxs-lookup"><span data-stu-id="f242a-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="f242a-103">停止の影響を受ける可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f242a-103">You might be impacted by an outage.</span></span> <span data-ttu-id="f242a-104">「[Azure 正常性状態](https://status.azure.com/status/history/)」で、継続的に停止していないか確認してください。</span><span class="sxs-lookup"><span data-stu-id="f242a-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="f242a-105">すべてのアクティブな Azure セッションからログアウトしてください。</span><span class="sxs-lookup"><span data-stu-id="f242a-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="f242a-106">Web ブラウザーのプライベート モードまたはシークレット モードを開始します。</span><span class="sxs-lookup"><span data-stu-id="f242a-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="f242a-107">また、上記の操作でも機能しない場合は、ブラウザーの更新、別のブラウザーの使用、キャッシュ Cookie の削除などを試すこともできます。</span><span class="sxs-lookup"><span data-stu-id="f242a-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="f242a-108">詳細については、「[サインインの問題に関するトラブルシューティング](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f242a-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="f242a-109">**サブスクリプションにアクセスできない**</span><span class="sxs-lookup"><span data-stu-id="f242a-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="f242a-110">[[Azure portal](https://portal.azure.com/)] で、右上のアカウントから正しい Azure ディレクトリが選択されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="f242a-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="f242a-111">[[Azure アカウント センター](https://account.windowsazure.com/Subscriptions)] で、アカウントを使用しているのがアカウント管理者であることを確認します。</span><span class="sxs-lookup"><span data-stu-id="f242a-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="f242a-112">詳細については、「[サブスクリプションが見つからない場合のトラブルシューティング](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f242a-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="f242a-113">**請求履歴にアクセスできない**</span><span class="sxs-lookup"><span data-stu-id="f242a-113">**Unable to access billing history**</span></span>

<span data-ttu-id="f242a-114">アカウント管理者は、「[新しいユーザーを追加または削除](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support)」で、請求情報にアクセスするユーザーが Azure Active Directory にゲスト ユーザーとして追加されたことを確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f242a-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="f242a-115">ユーザーは、「[ユーザーにロールを割り当てる](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support)」でグローバル管理者ロールが割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f242a-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="f242a-116">これを投稿し、「[請求へのアクセスを許可](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)」で RBAC ポリシーを使用してユーザーに請求へのアクセス許可を割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="f242a-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="f242a-117">**おすすめのドキュメント**</span><span class="sxs-lookup"><span data-stu-id="f242a-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="f242a-118">Azure サブスクリプションの管理にサインインできない</span><span class="sxs-lookup"><span data-stu-id="f242a-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)