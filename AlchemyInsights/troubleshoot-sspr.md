---
title: SSPR のトラブルシューティング
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430410"
---
# <a name="troubleshoot-sspr"></a><span data-ttu-id="f9ce8-102">SSPR のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="f9ce8-102">Troubleshoot SSPR</span></span>

<span data-ttu-id="f9ce8-103">**パスワードのリセットの構成に問題がある**</span><span class="sxs-lookup"><span data-stu-id="f9ce8-103">**I'm having trouble configuring password reset**</span></span>

- <span data-ttu-id="f9ce8-104">お客様が管理者であり、セルフサービスによるパスワードのリセットを有効にする方法を探している場合は、「[SSPR を有効にするためのチュートリアル](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)」を参照して、組織のパスワードのリセットを構成してください。</span><span class="sxs-lookup"><span data-stu-id="f9ce8-104">If you are administrator and looking for how to enable self-service password reset, see [Tutorial enable SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), to configure password reset for your organization.</span></span> <span data-ttu-id="f9ce8-105">「[ライセンス要件](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)」もご確認ください。</span><span class="sxs-lookup"><span data-stu-id="f9ce8-105">You may also want to review the [licensing requirements](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span> <span data-ttu-id="f9ce8-106">組織内で少なくとも 1 つのライセンスが割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f9ce8-106">You must have at least one license assigned in your organization.</span></span>
    - <span data-ttu-id="f9ce8-107">**クラウド専用ユーザー** - 任意の Office 365 (O365) 有料 SKU または Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="f9ce8-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="f9ce8-108">**クラウドとオンプレミス ユーザー** - Azure AD Premium P1 または P2、Enterprise Mobility + Security (EMS)、または Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="f9ce8-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
- <span data-ttu-id="f9ce8-109">セルフサービスによるパスワードのリセットに関するその他の質問については、「[FAQ](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f9ce8-109">For additional questions about self-service password reset, review [our FAQ](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="f9ce8-110">**次のエラー メッセージが表示されます**</span><span class="sxs-lookup"><span data-stu-id="f9ce8-110">**I'm getting an error message**</span></span>

<span data-ttu-id="f9ce8-111">一般的なエラーとその解決策を見つけるには、以下の記事を参照してください。「[セルフサービスによるパスワードのリセットのトラブルシューティングを行う](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)」</span><span class="sxs-lookup"><span data-stu-id="f9ce8-111">Review this article to find common errors and their solutions: [Troubleshoot self-service password reset](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="f9ce8-112">**パスワードのリセット ポリシーに問題がある**</span><span class="sxs-lookup"><span data-stu-id="f9ce8-112">**I'm having a problem with my password reset policy**</span></span>

- <span data-ttu-id="f9ce8-113">パスワード のリセット ポリシーが期待どおりに動作しない場合、またはパスワードのリセット ポリシーについて質問がある場合は、「[Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)のパスワード ポリシーと制限」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f9ce8-113">If your password reset policy is not behaving as expected, or if you have questions about password reset policies, review this article: [Password policies and restrictions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="f9ce8-114">パスワード リセット ポリシーは、管理者には適用されません。</span><span class="sxs-lookup"><span data-stu-id="f9ce8-114">Password reset policies do not apply to administrators.</span></span> <span data-ttu-id="f9ce8-115">Microsoft は Azure 管理者の役割に、強力な既定の 2 ゲート パスワード リセット ポリシーを適用しています。</span><span class="sxs-lookup"><span data-stu-id="f9ce8-115">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role.</span></span> <span data-ttu-id="f9ce8-116">管理者ではないユーザーでテストを行うようにしてください。</span><span class="sxs-lookup"><span data-stu-id="f9ce8-116">Make sure that you are testing with a user who is not an administrator.</span></span> <span data-ttu-id="f9ce8-117">管理者のリセット ポリシーの詳細については、「[管理者のリセット ポリシーの違い](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f9ce8-117">For more information on the administrator reset policy, see this article: [Administrator reset policy differences](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).</span></span>

<span data-ttu-id="f9ce8-118">**ユーザーにパスワードのリセットに関する追加のセキュリティ情報を登録させない**</span><span class="sxs-lookup"><span data-stu-id="f9ce8-118">**I don't want my users to register additional security info for password reset**</span></span>

<span data-ttu-id="f9ce8-119">API、PowerShell、または Azure AD Connect を使用して、ユーザーのデータ (メールと電話の属性) を事前に設定することができます。</span><span class="sxs-lookup"><span data-stu-id="f9ce8-119">You can pre-populate data (email and phone attributes) for your users using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="f9ce8-120">具体的な方法については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f9ce8-120">To learn how read:</span></span>

- [<span data-ttu-id="f9ce8-121">ユーザーに登録を求めることなくパスワードのリセットを展開する</span><span class="sxs-lookup"><span data-stu-id="f9ce8-121">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [<span data-ttu-id="f9ce8-122">パスワードのリセットで使用されるデータ</span><span class="sxs-lookup"><span data-stu-id="f9ce8-122">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="f9ce8-123">**ユーザーにパスワードの再設定のために追加のセキュリティ情報を登録してもらいたい**</span><span class="sxs-lookup"><span data-stu-id="f9ce8-123">**I want my users to register their additional security info for password reset**</span></span>

1. <span data-ttu-id="f9ce8-124">ユーザーを [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info) に誘導して、セルフサービスによるパスワードのリセットのためのセキュリティ情報を登録してもらいます。</span><span class="sxs-lookup"><span data-stu-id="f9ce8-124">Have your users register their security info for self service password reset by directing them to [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).</span></span>
1. <span data-ttu-id="f9ce8-125">(ユーザーまたは管理者によって) ユーザーのデータが入力されたら、ユーザーに [aka.ms/sspr](https://passwordreset.microsoftonline.com/) に誘導し、ユーザーが自分でパスワードをリセットできるようにします。</span><span class="sxs-lookup"><span data-stu-id="f9ce8-125">After data is populated for the user (by the user or by the admin), direct your user to [aka.ms/sspr](https://passwordreset.microsoftonline.com/) so your users can be empowered to reset their own passwords.</span></span>
1. <span data-ttu-id="f9ce8-126">ユーザーに引き続き問題が発生する場合は、**フェデレーション** ユーザーまたは **パスワード ハッシュが同期された** ユーザーである可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f9ce8-126">If users are still experiencing problems they are most likely **federated** or **password hash synched** users.</span></span> <span data-ttu-id="f9ce8-127">つまり、パスワード Writeback サービスに問題がある可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f9ce8-127">This means there is likely a problem with the Password Writeback service.</span></span>