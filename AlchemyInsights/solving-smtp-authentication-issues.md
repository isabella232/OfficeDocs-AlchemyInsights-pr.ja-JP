---
title: SMTP 認証の有効化とトラブルシューティング
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077656"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="c5695-102">SMTP 認証の有効化とトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="c5695-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="c5695-103">メールボックスの SMTP 認証を有効にしたい場合や、Microsoft 365 でデバイスやアプリケーションを認証してメールを中継しようとすると、5.7.57 または 5.7.3、5.7.139 のコードを含む「未認証のクライアント」、「認証は失敗しました」、「SmtpClientAuthentication」エラーが発生する場合は、以下の 3 つのアクションを実行して問題を解決してください。</span><span class="sxs-lookup"><span data-stu-id="c5695-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="c5695-104">「**セキュリティの既定値を有効にする**」を「**いいえ**」に切り替えて、「[Azure セキュリティの既定値](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)」を無効にします。</span><span class="sxs-lookup"><span data-stu-id="c5695-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="c5695-105">a.</span><span class="sxs-lookup"><span data-stu-id="c5695-105">a.</span></span> <span data-ttu-id="c5695-106">Azure ポータルにセキュリティ管理者、条件付きアクセス管理者、またはグローバル管理者としてサインインします。</span><span class="sxs-lookup"><span data-stu-id="c5695-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="c5695-107">b.</span><span class="sxs-lookup"><span data-stu-id="c5695-107">b.</span></span> <span data-ttu-id="c5695-108">[Azure Active Directory] >  **[プロパティ]** の順に移動します。</span><span class="sxs-lookup"><span data-stu-id="c5695-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="c5695-109">c.</span><span class="sxs-lookup"><span data-stu-id="c5695-109">c.</span></span> <span data-ttu-id="c5695-110">**[セキュリティの既定値を管理]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="c5695-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="c5695-111">d.</span><span class="sxs-lookup"><span data-stu-id="c5695-111">d.</span></span> <span data-ttu-id="c5695-112">**[セキュリティの既定値を有効にする]** を **[いいえ]** に設定します。</span><span class="sxs-lookup"><span data-stu-id="c5695-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="c5695-113">e.</span><span class="sxs-lookup"><span data-stu-id="c5695-113">e.</span></span> <span data-ttu-id="c5695-114">**[保存]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="c5695-114">Select **Save**.</span></span>

2. <span data-ttu-id="c5695-115">ライセンス付与済みのメールボックスで、[[クライアント SMTP 送信]](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) を有効にします。</span><span class="sxs-lookup"><span data-stu-id="c5695-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="c5695-116">a.</span><span class="sxs-lookup"><span data-stu-id="c5695-116">a.</span></span> <span data-ttu-id="c5695-117">Microsoft 365 管理センターから **[アクティブなユーザー]** に移動し、ユーザーを選択します。</span><span class="sxs-lookup"><span data-stu-id="c5695-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="c5695-118">b.</span><span class="sxs-lookup"><span data-stu-id="c5695-118">b.</span></span> <span data-ttu-id="c5695-119">[メール] タブを開き、**メール アプリ** の下にある **[メールアプリの管理]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="c5695-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="c5695-120">d.</span><span class="sxs-lookup"><span data-stu-id="c5695-120">d.</span></span> <span data-ttu-id="c5695-121">**[認証済み SMTP]** チェックボックスがオン (有効) になっていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="c5695-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="c5695-122">e.</span><span class="sxs-lookup"><span data-stu-id="c5695-122">e.</span></span> <span data-ttu-id="c5695-123">[**変更の保存**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c5695-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="c5695-124">ライセンス付与されたメールボックスで[多要素認証 (MFA) を無効にします](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa)。</span><span class="sxs-lookup"><span data-stu-id="c5695-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="c5695-125">a.</span><span class="sxs-lookup"><span data-stu-id="c5695-125">a.</span></span> <span data-ttu-id="c5695-126">Microsoft 365 管理センターに移動し、左側のナビゲーション メニューで、[**ユーザー** > **アクティブユーザー**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="c5695-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="c5695-127">b.</span><span class="sxs-lookup"><span data-stu-id="c5695-127">b.</span></span> <span data-ttu-id="c5695-128">**[多要素認証]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="c5695-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="c5695-129">c.</span><span class="sxs-lookup"><span data-stu-id="c5695-129">c.</span></span> <span data-ttu-id="c5695-130">ユーザーを選択し、**[多要素認証]** を無効にします。</span><span class="sxs-lookup"><span data-stu-id="c5695-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
