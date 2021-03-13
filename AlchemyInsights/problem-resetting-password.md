---
title: パスワードのリセットに関する問題
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696546"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="55454-102">パスワードのリセットに関する問題</span><span class="sxs-lookup"><span data-stu-id="55454-102">Problems resetting password</span></span>

<span data-ttu-id="55454-103">パスワードをリセットするときに発生する可能性がある問題と、考えられる解決策を次に示します。</span><span class="sxs-lookup"><span data-stu-id="55454-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="55454-104">**他のカテゴリで取り上げられていない、パスワードのリセットに関する問題が発生する**</span><span class="sxs-lookup"><span data-stu-id="55454-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

- <span data-ttu-id="55454-105">パスワードをリセットする権限があることを確認します。</span><span class="sxs-lookup"><span data-stu-id="55454-105">Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="55454-106">グローバル管理者、パスワード管理者、およびユーザー管理者のみがユーザー パスワードをリセットできます。</span><span class="sxs-lookup"><span data-stu-id="55454-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="55454-107">グローバル管理者は、他の特権を持つ管理者のパスワードをリセットすることもできます。</span><span class="sxs-lookup"><span data-stu-id="55454-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="55454-108">ライセンス要件を理解していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="55454-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="55454-109">組織内で少なくとも 1 つのライセンスが割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="55454-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="55454-110">クラウド専用ユーザー - 任意の Office 365 (O365) 有料 SKU または Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="55454-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="55454-111">クラウドとオンプレミス ユーザー - Azure AD Premium P1 または P2、Enterprise Mobility + Security (EMS)、または Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="55454-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="55454-112">ライセンス要件の詳細については、「[Azure AD セルフサービスによるパスワードのリセットのライセンス要件](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)」の記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="55454-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="55454-113">**設定したパスワード リセット ポリシーのテストで問題が発生している**</span><span class="sxs-lookup"><span data-stu-id="55454-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="55454-114">最近適用したポリシーは、すべてのデータ センターとエンド ポイント間で複製するため、数分かかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="55454-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="55454-115">データ センターからの物理的な距離も、変更が適用されるスピードに影響します。</span><span class="sxs-lookup"><span data-stu-id="55454-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="55454-116">管理者ではなくエンド ユーザーとテストし、小さなユーザーの一群をパイロットします。</span><span class="sxs-lookup"><span data-stu-id="55454-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="55454-117">Azure ポータルで構成されたポリシーはエンドユーザーにのみ適用され、管理者には適用されません。</span><span class="sxs-lookup"><span data-stu-id="55454-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="55454-118">Microsoft は、Azure 管理者ロールに強力な既定の 2 段階パスワード リセット ポリシーを適用しています (例: グローバル管理者、ヘルプデスク管理者、パスワード管理者など)。</span><span class="sxs-lookup"><span data-stu-id="55454-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="55454-119">「[管理者のポリシー](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)」の詳細については、次をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="55454-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="55454-120">**パスワードのリセットを展開したいが、ユーザーに追加のセキュリティ情報の登録を許可したくない**</span><span class="sxs-lookup"><span data-stu-id="55454-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="55454-121">ユーザーのために事前入力されているため、ユーザーが入力する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="55454-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="55454-122">- 管理者は、組織にパスワードのリセットを展開する前に、ユーザーの電話とメールのプロパティを設定できます。</span><span class="sxs-lookup"><span data-stu-id="55454-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="55454-123">これは、API、PowerShell、または Azure AD Connect を使用して行うことができます。</span><span class="sxs-lookup"><span data-stu-id="55454-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="55454-124">詳細情報については、こちらを参照してください。</span><span class="sxs-lookup"><span data-stu-id="55454-124">More information here:</span></span>
- [<span data-ttu-id="55454-125">ユーザーに登録を求めることなくパスワードのリセットを展開する</span><span class="sxs-lookup"><span data-stu-id="55454-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="55454-126">パスワードのリセットで使用されるデータ</span><span class="sxs-lookup"><span data-stu-id="55454-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="55454-127">**[パスワードのリセット] ボタンが灰色表示されています**</span><span class="sxs-lookup"><span data-stu-id="55454-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="55454-128">このユーザーのパスワードをリセットする権限がありません。</span><span class="sxs-lookup"><span data-stu-id="55454-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="55454-129">グローバル管理者、パスワード管理者、およびユーザー管理者のみがユーザー パスワードをリセットできます。</span><span class="sxs-lookup"><span data-stu-id="55454-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="55454-130">グローバル管理者は、他の特権を持つ管理者のパスワードをリセットすることもできます。</span><span class="sxs-lookup"><span data-stu-id="55454-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="55454-131">**パスワード リセット ブレードが表示されていません**</span><span class="sxs-lookup"><span data-stu-id="55454-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="55454-132">パスワードをリセットする権限がありません。</span><span class="sxs-lookup"><span data-stu-id="55454-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="55454-133">グローバル管理者、パスワード管理者、およびユーザー管理者のみがユーザー パスワードをリセットできます。</span><span class="sxs-lookup"><span data-stu-id="55454-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="55454-134">グローバル管理者は、他の特権を持つ管理者のパスワードをリセットすることもできます。</span><span class="sxs-lookup"><span data-stu-id="55454-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="55454-135">**[パスワードのリセット] にオンプレミス統合ブレードが表示されていません**</span><span class="sxs-lookup"><span data-stu-id="55454-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="55454-136">オンプレミス統合ブレードは、ハイブリッド環境だけで表示されます。つまり、パスワードの書き戻しを使用してオンプレミス ユーザーのパスワードを操作します。</span><span class="sxs-lookup"><span data-stu-id="55454-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="55454-137">次の場合、このブレードは表示されません。</span><span class="sxs-lookup"><span data-stu-id="55454-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="55454-138">パスワードの書き戻しを使用していない</span><span class="sxs-lookup"><span data-stu-id="55454-138">You are not using password writeback</span></span>
    - <span data-ttu-id="55454-139">パスワードの書き戻しのインストール/接続に問題がある</span><span class="sxs-lookup"><span data-stu-id="55454-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="55454-140">Azure AD Connect のインストール/接続に問題がある</span><span class="sxs-lookup"><span data-stu-id="55454-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="55454-141">パスワードの書き戻しに関する問題のトラブルシューティングの手順については、「[パスワードの書き戻しに関するトラブルシューティング](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)」セクションを参照してください。</span><span class="sxs-lookup"><span data-stu-id="55454-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="55454-142">**ユーザーのパスワードをリセットする方法がわかりません**</span><span class="sxs-lookup"><span data-stu-id="55454-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="55454-143">パスワードをリセットできる適切な管理者として Azure portal にサインインします。</span><span class="sxs-lookup"><span data-stu-id="55454-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="55454-144">[ユーザーおよびグループ] ブレードに移動し、**[すべてのユーザー]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="55454-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="55454-145">一覧からユーザーを選択します。</span><span class="sxs-lookup"><span data-stu-id="55454-145">Select a user from the list.</span></span>
1. <span data-ttu-id="55454-146">選択したユーザーに対して、[**概要**] を選択し、コマンド バーで [**パスワードのリセット**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="55454-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="55454-147">画面の指示に従います。</span><span class="sxs-lookup"><span data-stu-id="55454-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="55454-148">Azure portal で実行されるリセットのみ、パスワードの書き戻しをサポートします。</span><span class="sxs-lookup"><span data-stu-id="55454-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="55454-149">**Office 365 管理ポータルまたは Office 365 モバイル アプリケーションからオンプレミス ユーザーのパスワードをリセットしましたが、ユーザーがまだサインインできません**</span><span class="sxs-lookup"><span data-stu-id="55454-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="55454-150">このポータルでは、パスワードの書き戻しはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="55454-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="55454-151">Azure portal - portal.azure.com でユーザーのパスワードをリセットします。</span><span class="sxs-lookup"><span data-stu-id="55454-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>

