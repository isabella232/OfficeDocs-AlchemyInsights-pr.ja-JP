---
title: 外部設定の管理
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/17/2021
ms.locfileid: "50294492"
---
# <a name="managing-external-settings"></a><span data-ttu-id="a2e46-102">外部設定の管理</span><span class="sxs-lookup"><span data-stu-id="a2e46-102">Managing External Settings</span></span>

<span data-ttu-id="a2e46-103">**アナウンス**</span><span class="sxs-lookup"><span data-stu-id="a2e46-103">**Announcement**</span></span>

- <span data-ttu-id="a2e46-104">[2021 年 1 月 4 日以降、Google からの Web View サインイン サポートの廃止](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support)。</span><span class="sxs-lookup"><span data-stu-id="a2e46-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span></span> <span data-ttu-id="a2e46-105">互換性のテストに関する Google のガイダンスに従って、アプリが影響を受けるかどうかをテストします</span><span class="sxs-lookup"><span data-stu-id="a2e46-105">Test whether your apps are affected by following Google’s guidance on testing compatibility</span></span>
- <span data-ttu-id="a2e46-106">コンシューマー Google アカウントでユーザーにサインインするときは、システム Web ビューまたはシステム ブラウザーを使用していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="a2e46-106">Make sure to use the system webview or the system browser when signing in your users with consumer Google accounts</span></span>

<span data-ttu-id="a2e46-107">**招待設定の管理**</span><span class="sxs-lookup"><span data-stu-id="a2e46-107">**Manage Invitation Settings**</span></span>

<span data-ttu-id="a2e46-108">適切な人が招待状を送信できるように[外部コラボレーション設定を構成したことを確認します](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="a2e46-108">Confirm that you have [configured the external collaboration settings](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) to allow the appropriate people to send invitations.</span></span>

<span data-ttu-id="a2e46-109">**ゲスト ユーザーのアクセス許可を管理する**</span><span class="sxs-lookup"><span data-stu-id="a2e46-109">**Manage Guest User Access Permissions**</span></span>

1. <span data-ttu-id="a2e46-110">グローバル管理者は、[外部コラボレーション設定] ページでゲスト アクセス許可を構成することにより、Azure portal を介してディレクトリ内のゲスト アクセス許可を管理できます。</span><span class="sxs-lookup"><span data-stu-id="a2e46-110">Global admins can manage guest access permissions in the directory through the Azure portal by configuring the guest access permissions on the External Collaboration Settings page.</span></span> <span data-ttu-id="a2e46-111">[この設定の詳細をご覧ください](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="a2e46-111">[Learn more about this setting](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
2. <span data-ttu-id="a2e46-112">ゲストが Teams や SharePoint などのアプリにアクセスできるようにする場合は、ゲスト アクセスを許可するようにそれらのアプリが構成されていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="a2e46-112">If you would like your guests to access apps such as Teams or SharePoint, confirm that you've configured those apps to allow guest access.</span></span> <span data-ttu-id="a2e46-113">[Teams の設定](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support)と [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support) についての詳細をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="a2e46-113">Learn more about the [Teams settings](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) and [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="a2e46-114">**共有招待状:**</span><span class="sxs-lookup"><span data-stu-id="a2e46-114">**Configuring invitations:**</span></span>

- [<span data-ttu-id="a2e46-115">B2B の外部コラボレーションを有効にしてゲストを招待できるユーザーを管理する</span><span class="sxs-lookup"><span data-stu-id="a2e46-115">Enable B2B external collaboration and manage who can invite guests</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="a2e46-116">ユーザーに対する特定組織からの招待を許可またはブロックする</span><span class="sxs-lookup"><span data-stu-id="a2e46-116">Allow or block invitations to users from specific organizations</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="a2e46-117">**許可された ID プロバイダーの構成:**</span><span class="sxs-lookup"><span data-stu-id="a2e46-117">**Configuring allowed identity providers:**</span></span>

- [<span data-ttu-id="a2e46-118">Google フェデレーション</span><span class="sxs-lookup"><span data-stu-id="a2e46-118">Google Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="a2e46-119">直接フェデレーション</span><span class="sxs-lookup"><span data-stu-id="a2e46-119">Direct Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="a2e46-120">ワンタイム パスコード認証をメールで送信する</span><span class="sxs-lookup"><span data-stu-id="a2e46-120">Email one-time Passcode Authentication</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
