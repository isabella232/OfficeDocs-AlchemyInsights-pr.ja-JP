---
title: ユーザーによるパスワードのリセットのセットアップ
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9357"
- "9003259"
ms.openlocfilehash: 0a771c43b308794af1efd55b9c185b2dcff71700
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2021
ms.locfileid: "50696404"
---
# <a name="user-reset-password-setup"></a><span data-ttu-id="f1b20-102">ユーザーによるパスワードのリセットのセットアップ</span><span class="sxs-lookup"><span data-stu-id="f1b20-102">User reset password setup</span></span>

<span data-ttu-id="f1b20-103">**ユーザーがパスワードをリセットする方法**</span><span class="sxs-lookup"><span data-stu-id="f1b20-103">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="f1b20-104">ユーザーは、パスワードをリセットする前に、[aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info) でセルフサービスによるパスワードのリセットに登録する必要があります。 </span><span class="sxs-lookup"><span data-stu-id="f1b20-104">Users need to register for self-service password reset at [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info) before they can reset their passwords.</span></span> <span data-ttu-id="f1b20-105">ユーザーが登録すると、「[職場または学校のパスワードをリセットする](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-update-your-own-password)」の手順に従ってパスワードをリセットできます。</span><span class="sxs-lookup"><span data-stu-id="f1b20-105">Once a user has registered, the users can follow the instructions in [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-update-your-own-password) to reset their passwords.</span></span>

<span data-ttu-id="f1b20-106">**ユーザーがパスワードを変更する方法**</span><span class="sxs-lookup"><span data-stu-id="f1b20-106">**How do my users change their passwords?**</span></span>

<span data-ttu-id="f1b20-107">ユーザーは、「[パスワードを変更する方法](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-update-your-own-password)」の手順に従ってパスワードを変更できます: </span><span class="sxs-lookup"><span data-stu-id="f1b20-107">Users can follow the steps in [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-update-your-own-password) to change their passwords.</span></span>

<span data-ttu-id="f1b20-108">**パスワードを変更またはリセットすると、ユーザーにエラーが発生します**</span><span class="sxs-lookup"><span data-stu-id="f1b20-108">**My users are getting an error when changing or resetting their passwords**</span></span>

<span data-ttu-id="f1b20-109">ユーザーがパスワードをリセットしようとしたときに発生する一般的な問題については、「[一般的な問題とその解決策](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-update-your-own-password)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="f1b20-109">See [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-update-your-own-password) for information on common problems that can arise when users are trying to reset their passwords.</span></span>

<span data-ttu-id="f1b20-110">**ユーザーがセルフサービスによるパスワードのリセットに登録する方法**</span><span class="sxs-lookup"><span data-stu-id="f1b20-110">**How do my users register for self-service password reset?**</span></span>

<span data-ttu-id="f1b20-111">セルフサービス によるパスワードのリセットに登録するには、次の方法があります。</span><span class="sxs-lookup"><span data-stu-id="f1b20-111">To register for self-service password reset:</span></span>

- <span data-ttu-id="f1b20-112">ユーザーは、「[セルフサービスによるパスワードのリセットを登録する](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register)」の手順に従って操作を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="f1b20-112">Users can follow the steps in [Register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register).</span></span>
- <span data-ttu-id="f1b20-113">統合された登録がユーザーに対して有効になっている場合は、「[セキュリティ情報 (プレビュー)の概要](https://docs.microsoft.com/azure/active-directory/user-help/security-info-setup-signin)」に記載されているチュートリアルに従って操作を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="f1b20-113">Users can follow the tutorials listed in [Security info (preview) overview](https://docs.microsoft.com/azure/active-directory/user-help/security-info-setup-signin) if they have been enabled for converged registration.</span></span>

<span data-ttu-id="f1b20-114">**セルフサービスによるパスワードのリセットと多要素認証のための、組み合わされたセキュリティ情報の登録を有効にする方法**</span><span class="sxs-lookup"><span data-stu-id="f1b20-114">**How do I enable combined security info registration for self-service password reset and Multi-Factor Authentication?**</span></span>

<span data-ttu-id="f1b20-115">セキュリティ情報の登録の組み合わせと、ユーザーに対して登録を有効にする方法については、「[SSPR と MFA の登録の組み合わせ - Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-registration-mfa-sspr-combined)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f1b20-115">For information about combined security info registration and how to enable it for your users, see [Combined registration for SSPR and MFA - Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-registration-mfa-sspr-combined).</span></span>

<span data-ttu-id="f1b20-116">**ユーザーにセルフサービスによるパスワードのリセットの登録を要求する方法**</span><span class="sxs-lookup"><span data-stu-id="f1b20-116">**How do I require my users to register for self-service password reset?**</span></span>

<span data-ttu-id="f1b20-117">サインイン時にユーザーに登録を要求するには、「[パスワードリセットのしくみ: 登録](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-howitworks)」の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="f1b20-117">To require users to register when they sign in, follow the steps in [How password reset works: Registration](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-howitworks).</span></span>

<span data-ttu-id="f1b20-118">機能のリクエストを送信するには、[aka.ms/sspruservoice](https://feedback.azure.com/forums/169401-azure-active-directory/category/166251-self-service-password-reset) ページにアクセスしてください。</span><span class="sxs-lookup"><span data-stu-id="f1b20-118">To submit a feature request, go to [aka.ms/sspruservoice](https://feedback.azure.com/forums/169401-azure-active-directory/category/166251-self-service-password-reset)</span></span>



 












