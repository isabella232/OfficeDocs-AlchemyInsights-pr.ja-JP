---
title: パスワード ポリシー
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751144"
---
# <a name="password-policies"></a><span data-ttu-id="bf567-102">パスワード ポリシー</span><span class="sxs-lookup"><span data-stu-id="bf567-102">Password policies</span></span>

<span data-ttu-id="bf567-103">**ユーザーのパスワード ポリシーに問題があります**</span><span class="sxs-lookup"><span data-stu-id="bf567-103">**I'm having problems with the password policy for a user**</span></span>

- <span data-ttu-id="bf567-104">ユーザーのパスワード ポリシーは、ユーザーがクラウドのみであるかオンプレミスであるかによって異なります。</span><span class="sxs-lookup"><span data-stu-id="bf567-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span></span>
- <span data-ttu-id="bf567-105">クラウドのみのユーザーは、この記事の要件を満たすパスワードを選択する必要があります: 「[クラウド ユーザー アカウントにのみ適用されるパスワード ポリシー](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)」</span><span class="sxs-lookup"><span data-stu-id="bf567-105">Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- <span data-ttu-id="bf567-106">オンプレミス ユーザーは、オンプレミスの要件を満たすパスワードを選択する必要があります。</span><span class="sxs-lookup"><span data-stu-id="bf567-106">On-premises users must choose a password that meets the on-premises requirements.</span></span> <span data-ttu-id="bf567-107">オンプレミス ユーザーがパスワードを設定できない場合は、オンプレミスの要件を確認してください。</span><span class="sxs-lookup"><span data-stu-id="bf567-107">If an on-premises user is unable to set their password, check your on-premises requirements.</span></span>

<span data-ttu-id="bf567-108">**パスワードの有効期限ポリシーを設定または確認する方法がわかりません**</span><span class="sxs-lookup"><span data-stu-id="bf567-108">**I don't know how to set or check password expiration policies**</span></span>

- <span data-ttu-id="bf567-109">PowerShell を使用して、テナント内のクラウド ユーザーの有効期限ポリシーを設定および確認できます。</span><span class="sxs-lookup"><span data-stu-id="bf567-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span></span> <span data-ttu-id="bf567-110">この記事の指示に従ってください: 「[PowerShell を使用してパスワード ポリシーを設定または確認する](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)」</span><span class="sxs-lookup"><span data-stu-id="bf567-110">Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span></span>
- <span data-ttu-id="bf567-111">オンプレミス ユーザーのパスワード有効期限ポリシーは、オンプレミス AD で設定されます。</span><span class="sxs-lookup"><span data-stu-id="bf567-111">The password expiration policy for on-premises users is set in your on-premises AD.</span></span>

<span data-ttu-id="bf567-112">**その他の便利なリンク:**</span><span class="sxs-lookup"><span data-stu-id="bf567-112">**Other Helpful links:**</span></span>
- [<span data-ttu-id="bf567-113">パスワード リセットの概要</span><span class="sxs-lookup"><span data-stu-id="bf567-113">Getting Started with Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [<span data-ttu-id="bf567-114">管理者が開始したパスワード リセットのトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="bf567-114">Troubleshoot Administrator-initiated Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
