---
title: ゲスト ユーザーに関する問題のトラブルシューティング
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901742"
---
# <a name="troubleshoot-guest-user-issues"></a><span data-ttu-id="b5bad-102">ゲスト ユーザーに関する問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="b5bad-102">Troubleshoot guest user issues</span></span>

1. <span data-ttu-id="b5bad-103">アプリケーションへのゲストアクセスの管理に関するガイダンスについては、「[Azure AD のアクセス レビューによるゲスト アクセスの管理](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b5bad-103">For guidance on managing guest access to applications, see [Manage guest access with Azure AD access reviews](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).</span></span>
1. <span data-ttu-id="b5bad-104">[Azure portal のディレクトリにゲストユーザーを追加する](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): このクイックスタートでは、Azure portal を介して新しいゲストユーザーを Azure AD ディレクトリに追加し、招待状を送信して、ゲストユーザーの招待状の引き換えプロセスがどのようになるかを確認します。</span><span class="sxs-lookup"><span data-stu-id="b5bad-104">[Add guest users to your directory in the Azure portal](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): In this quickstart, you'll add a new guest user to your Azure AD directory via the Azure portal, send an invitation, and see what the guest user's invitation redemption process looks like.</span></span>
1. <span data-ttu-id="b5bad-105">[PowerShell を使用してゲストユーザーを追加する](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): このクイックスタートでは、New-AzureADMSInvitation コマンドを使用して、1 人のゲストユーザーを Azure テナントに追加します。</span><span class="sxs-lookup"><span data-stu-id="b5bad-105">[Add a guest user with PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): In this quickstart, you’ll use the New-AzureADMSInvitation command to add one guest user to your Azure tenant.</span></span>
1. <span data-ttu-id="b5bad-106">Azure ポータル内からまたは PowerShell を使用して、Azure Active Directory (Azure AD) のエンタープライズ アプリケーションにユーザーとグループを割り当てる方法については、「[Azure Active Directory でのアプリのユーザー割り当ての管理](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b5bad-106">To learn how to assign users, and groups, to enterprise applications in Azure Active Directory (Azure AD), either from within the Azure portal or by using PowerShell, see [Manage user assignment for an app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).</span></span> 
1. <span data-ttu-id="b5bad-107">Azure Active Directory (Azure AD) B2B コラボレーションは、Azure ADと統合するほとんどのアプリで機能します。</span><span class="sxs-lookup"><span data-stu-id="b5bad-107">Azure Active Directory (Azure AD) B2B collaboration works with most apps that integrate with Azure AD.</span></span> <span data-ttu-id="b5bad-108">この[記事](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)では、Azure AD B2B で使用するためにいくつかの一般的な SaaS アプリを構成する手順について説明します。</span><span class="sxs-lookup"><span data-stu-id="b5bad-108">In this [article](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps), we walk through instructions for configuring some popular SaaS apps for use with Azure AD B2B.</span></span>
1. <span data-ttu-id="b5bad-109">Azure Active Directory (Azure AD) B2B コラボレーション機能を使用してパートナー組織からゲストユーザーを Azure AD に招待する組織として、これらの B2B ユーザーにオンプレミス アプリへのアクセスを提供できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="b5bad-109">As an organization that uses Azure Active Directory (Azure AD) B2B collaboration capabilities to invite guest users from partner organizations to your Azure AD, you can now provide these B2B users access to on-premises apps.</span></span> <span data-ttu-id="b5bad-110">これらのオンプレミス アプリは、SAML ベースの認証または Kerberos 制約付き委任 (KCD) を使用した統合 Windows 認証 (IWA) を使用できます。</span><span class="sxs-lookup"><span data-stu-id="b5bad-110">These on-premises apps can use SAML-based authentication or Integrated Windows Authentication (IWA) with Kerberos constrained delegation (KCD).</span></span> <span data-ttu-id="b5bad-111">詳細については、「[Azure AD の B2B ユーザーにオンプレミスのアプリケーションへのアクセスを許可する](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="b5bad-111">For more information, see [Grant B2B users in Azure AD access to your on-premises applications](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises).</span></span>
1. <span data-ttu-id="b5bad-112">[Azure AD B2B コラボレーションを使用して、ローカルで管理されているパートナー アカウントにクラウド リソースへのアクセスを許可する](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)方法を確認してください。</span><span class="sxs-lookup"><span data-stu-id="b5bad-112">Learn how to [grant locally-managed partner accounts access to cloud resources using Azure AD B2B collaboration](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud).</span></span>