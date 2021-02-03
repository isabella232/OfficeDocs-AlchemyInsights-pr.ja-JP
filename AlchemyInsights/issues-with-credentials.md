---
title: 資格情報に関する問題
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063734"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="3886e-102">資格情報に関する問題</span><span class="sxs-lookup"><span data-stu-id="3886e-102">Issues with credentials</span></span>

<span data-ttu-id="3886e-103">[Microsoft ID プラットフォームおよび OAuth 2.0 クライアント資格情報フロー](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)は、OAuth 2.0 クライアント資格情報付与フローに対して直接プログラムする方法を説明しています。</span><span class="sxs-lookup"><span data-stu-id="3886e-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="3886e-104">**アプリケーションのパスワードまたは証明書の資格情報を管理するする方法**</span><span class="sxs-lookup"><span data-stu-id="3886e-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="3886e-105">Azure CLI では、[az ad app 資格情報](https://docs.microsoft.com/cli/azure/ad/app/credential)を使用して、アプリケーションのパスワードまたは証明書の資格情報を削除、一覧表示、またはリセットできます。</span><span class="sxs-lookup"><span data-stu-id="3886e-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="3886e-106">**ユーザーがパスワードをリセットする方法**</span><span class="sxs-lookup"><span data-stu-id="3886e-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="3886e-107">ユーザーは、パスワードをリセットする前に、[セルフサービスによるパスワードのリセットに登録する](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register)必要があります。</span><span class="sxs-lookup"><span data-stu-id="3886e-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="3886e-108">ユーザーが登録すると、この記事の手順に従ってパスワードをリセットできます: [職場または学校のパスワードをリセットする](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)</span><span class="sxs-lookup"><span data-stu-id="3886e-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="3886e-109">**ユーザーがパスワードを変更する方法**</span><span class="sxs-lookup"><span data-stu-id="3886e-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="3886e-110">ユーザーは、この記事の手順に従ってパスワードを変更できます: [パスワードを変更する方法](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)</span><span class="sxs-lookup"><span data-stu-id="3886e-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="3886e-111">また、[2 段階認証のためにアプリ パスワードを管理する](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)こともできます。</span><span class="sxs-lookup"><span data-stu-id="3886e-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="3886e-112">**パスワードを変更またはリセットすると、ユーザーにエラーが発生します**</span><span class="sxs-lookup"><span data-stu-id="3886e-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="3886e-113">このリンクは、ユーザーがパスワードをリセットしようとしたときに発生する一般的な問題に関する情報を提供します: [一般的な問題とその解決策](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="3886e-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="3886e-114">**ユーザーのパスワードのリセット中に問題が発生しました**</span><span class="sxs-lookup"><span data-stu-id="3886e-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="3886e-115">パスワードをリセットする権限があることを確認します。</span><span class="sxs-lookup"><span data-stu-id="3886e-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="3886e-116">*グローバル、パスワード、およびユーザー管理者のみがユーザー パスワードをリセットできます。*</span><span class="sxs-lookup"><span data-stu-id="3886e-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="3886e-117">グローバル管理者は、他の特権を持つ管理者のパスワードをリセットすることもできます。</span><span class="sxs-lookup"><span data-stu-id="3886e-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="3886e-118">ライセンス要件を理解していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="3886e-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="3886e-119">組織内で少なくとも 1 つのライセンスが割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3886e-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="3886e-120">**クラウド専用ユーザー** - 任意の Office 365 (O365) 有料 SKU または Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="3886e-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="3886e-121">**クラウドとオンプレミス ユーザー** - Azure AD Premium P1 または P2、Enterprise Mobility + Security (EMS)、または Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="3886e-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="3886e-122">ライセンス要件の詳細については、「[Azure AD セルフサービスによるパスワードのリセットのライセンス要件](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3886e-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="3886e-123">ユーザーのパスワードをリセットするには、Azure AD でユーザーを検索します。</span><span class="sxs-lookup"><span data-stu-id="3886e-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="3886e-124">次に、そのユーザーの概要ブレードで、[パスワードのリセット] ボタンをクリックします。</span><span class="sxs-lookup"><span data-stu-id="3886e-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="3886e-125">**[パスワードのリセット] ボタンが灰色表示されています**</span><span class="sxs-lookup"><span data-stu-id="3886e-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="3886e-126">**この** ユーザーのパスワードをリセットする権限がありません。</span><span class="sxs-lookup"><span data-stu-id="3886e-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="3886e-127">*グローバル、パスワード、およびユーザー管理者のみがユーザー パスワードをリセットできます。*</span><span class="sxs-lookup"><span data-stu-id="3886e-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="3886e-128">グローバル管理者は、他の特権を持つ管理者のパスワードをリセットすることもできます。</span><span class="sxs-lookup"><span data-stu-id="3886e-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="3886e-129">**パスワード リセット ブレードが表示されていません**</span><span class="sxs-lookup"><span data-stu-id="3886e-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="3886e-130">パスワードをリセットする権限がありません。</span><span class="sxs-lookup"><span data-stu-id="3886e-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="3886e-131">*グローバル、パスワード、およびユーザー管理者のみがユーザー パスワードをリセットできます。*</span><span class="sxs-lookup"><span data-stu-id="3886e-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="3886e-132">グローバル管理者は、他の特権を持つ管理者のパスワードをリセットすることもできます。</span><span class="sxs-lookup"><span data-stu-id="3886e-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="3886e-133">**[パスワードのリセット] にオンプレミス統合ブレードが表示されていません**</span><span class="sxs-lookup"><span data-stu-id="3886e-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="3886e-134">オンプレミス統合ブレードは、ハイブリッド環境だけで表示されます。つまり、パスワードの書き戻しを使用してオンプレミス ユーザーのパスワードを操作します。</span><span class="sxs-lookup"><span data-stu-id="3886e-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="3886e-135">次の場合、このブレードは表示されません。</span><span class="sxs-lookup"><span data-stu-id="3886e-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="3886e-136">パスワードの書き戻しを使用していない</span><span class="sxs-lookup"><span data-stu-id="3886e-136">You are not using password writeback</span></span>
  - <span data-ttu-id="3886e-137">パスワードの書き戻しのインストール/接続に問題がある</span><span class="sxs-lookup"><span data-stu-id="3886e-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="3886e-138">Azure AD Connect のインストール/接続に問題がある</span><span class="sxs-lookup"><span data-stu-id="3886e-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="3886e-139">パスワードの書き戻しに関する問題のトラブルシューティングの手順については、「[パスワードの書き戻しに関するトラブルシューティング](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3886e-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="3886e-140">**ユーザーのパスワードをリセットする方法がわかりません**</span><span class="sxs-lookup"><span data-stu-id="3886e-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="3886e-141">パスワードをリセットできる適切な管理者として Azure portal にサインインします。</span><span class="sxs-lookup"><span data-stu-id="3886e-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="3886e-142">**[ユーザーおよびグループ]** ブレードに移動し、**[すべてのユーザー]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="3886e-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="3886e-143">一覧からユーザーを選択します。</span><span class="sxs-lookup"><span data-stu-id="3886e-143">Select a user from the list.</span></span>
4. <span data-ttu-id="3886e-144">選択したユーザーに対して、**[概要]** を選択し、コマンド バーで **[パスワードのリセット]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="3886e-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="3886e-145">**[パスワードのリセット]** ボタンを選択し、画面の指示に従います。</span><span class="sxs-lookup"><span data-stu-id="3886e-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="3886e-146">**Azure portal** で実行されるリセットのみ、パスワードの書き戻しをサポートします。</span><span class="sxs-lookup"><span data-stu-id="3886e-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="3886e-147">**Office 365 管理ポータルまたは Office 365 モバイル アプリケーションからオンプレミス ユーザーのパスワードをリセットしましたが、ユーザーがまだサインインできません**</span><span class="sxs-lookup"><span data-stu-id="3886e-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="3886e-148">このポータルでは、パスワードの書き戻しはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3886e-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="3886e-149">Azure portal でユーザーのパスワードをリセットします。</span><span class="sxs-lookup"><span data-stu-id="3886e-149">Reset the user's password again in the Azure portal.</span></span>
