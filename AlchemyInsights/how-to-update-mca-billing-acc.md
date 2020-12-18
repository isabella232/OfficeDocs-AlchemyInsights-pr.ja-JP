---
title: MCA に関連付けられている販売先住所および請求先住所の更新 - 推奨される手順
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004166"
- "7325"
ms.openlocfilehash: 8cdd2c64a95e88eb2fb4624c6e2696f77b75e198
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/11/2020
ms.locfileid: "49680548"
---
# <a name="update-sold-to-and-bill-to-address-associated-to-your-mca---recommended-steps"></a><span data-ttu-id="6dc2a-102">MCA に関連付けられている販売先住所および請求先住所の更新 - 推奨される手順</span><span class="sxs-lookup"><span data-stu-id="6dc2a-102">Update sold-to and bill-to address associated to your MCA - recommended steps</span></span>

<span data-ttu-id="6dc2a-103">Microsoft 顧客契約 (MCA) に関連付けられている販売先住所および請求先住所を更新できます。</span><span class="sxs-lookup"><span data-stu-id="6dc2a-103">You can update the sold-to and bill-to address associated to your Microsoft Customer Agreement (MCA).</span></span> 

> [!NOTE]
> <span data-ttu-id="6dc2a-104">Azure Active Directory のユーザー プロファイル情報を変更できるのは、ユーザー管理者だけです。</span><span class="sxs-lookup"><span data-stu-id="6dc2a-104">Only a user administrator can make changes to the Azure Active Directory user profile information.</span></span> <span data-ttu-id="6dc2a-105">ユーザーの管理者役割が割り当てられていない場合は、ユーザー管理者に問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="6dc2a-105">If you're not assigned the user administrator role, contact your user administrator.</span></span> <span data-ttu-id="6dc2a-106">ユーザーのプロファイルの変更の詳細については、「[Azure Active Directory を使用してユーザーのプロファイル情報を追加または更新する](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6dc2a-106">For more information about changing a user's profile, see [Add or update a user's profile information using Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal).</span></span>

<span data-ttu-id="6dc2a-107">**販売先住所**: 販売先住所は、課金アカウントの責任者である組織または個人の住所および連絡先情報です。</span><span class="sxs-lookup"><span data-stu-id="6dc2a-107">**Sold-to address** - The sold-to address is the address and the contact information of the organization or the individual, who is responsible for a billing account.</span></span> <span data-ttu-id="6dc2a-108">課金アカウント用に作成されたすべての請求書に表示されます。</span><span class="sxs-lookup"><span data-stu-id="6dc2a-108">It's displayed in all the invoices generated for the billing account.</span></span>

<span data-ttu-id="6dc2a-109">**請求先住所**: 請求先住所は、課金アカウントに対して生成された請求書の責任者である組織または個人の住所および連絡先情報です。</span><span class="sxs-lookup"><span data-stu-id="6dc2a-109">**Bill-to address** - The bill-to address is the address and the contact information of the organization or the individual, who is responsible for the invoices generated for a billing account.</span></span> <span data-ttu-id="6dc2a-110">MCA の課金アカウントの場合、課金プロファイルごとに請求先住所があり、請求プロファイル用に作成された請求書に表示されます。</span><span class="sxs-lookup"><span data-stu-id="6dc2a-110">For a billing account for an MCA, there's a bill-to address for each billing profile and it's displayed in the invoice generated for the billing profile.</span></span>

<span data-ttu-id="6dc2a-111">**MCA の課金アカウントの販売先住所を更新するには**:</span><span class="sxs-lookup"><span data-stu-id="6dc2a-111">**To update an MCA billing account sold-to address**:</span></span>

1. <span data-ttu-id="6dc2a-112">MCA の課金アカウントに対して所有者または投稿者ロールを持つメール アドレスを使用して、Azure ポータルにサインインします。</span><span class="sxs-lookup"><span data-stu-id="6dc2a-112">Sign in to the Azure portal using the email address, which has an owner or a contributor role on the billing account for an MCA.</span></span>
1. <span data-ttu-id="6dc2a-113">**[コストの管理** + **課金]** を検索します。</span><span class="sxs-lookup"><span data-stu-id="6dc2a-113">Search for **Cost Management** + **Billing**.</span></span>
1. <span data-ttu-id="6dc2a-114">**[プロパティ]** > **[販売先住所の更新]** の順にクリックします。</span><span class="sxs-lookup"><span data-stu-id="6dc2a-114">Click **Properties** > **Update sold-to**.</span></span>
1. <span data-ttu-id="6dc2a-115">新しい住所を入力し、**[保存]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="6dc2a-115">Enter the new address and click **Save**.</span></span>

<span data-ttu-id="6dc2a-116">一部のアカウントでは、販売先住所を更新する前に追加の確認が必要です。</span><span class="sxs-lookup"><span data-stu-id="6dc2a-116">Some accounts require additional verification before their sold-to address can be updated.</span></span> <span data-ttu-id="6dc2a-117">アカウントに手動承認が必要な場合は、Azure サポートに連絡するように求められます。</span><span class="sxs-lookup"><span data-stu-id="6dc2a-117">If your account requires manual approval, you'll be asked to contact Azure support.</span></span>

<span data-ttu-id="6dc2a-118">**MCA の課金アカウントの住所** を更新するには:</span><span class="sxs-lookup"><span data-stu-id="6dc2a-118">**To update an MCA billing account address**:</span></span> 

1. <span data-ttu-id="6dc2a-119">MCA の課金アカウントまたは MCA の課金プロファイルに対して所有者または投稿者ロールを持つメール アドレスを使用して、Azure ポータルにサインインします。</span><span class="sxs-lookup"><span data-stu-id="6dc2a-119">Sign in to the Azure portal using the email address, which has an owner or a contributor role on a billing account or a billing profile for an MCA.</span></span>
1. <span data-ttu-id="6dc2a-120">**[コストの管理** + **課金]** を検索します。</span><span class="sxs-lookup"><span data-stu-id="6dc2a-120">Search for **Cost Management** + **Billing**.</span></span>
1. <span data-ttu-id="6dc2a-121">**[課金プロファイル]** をクリックし、課金プロファイルを選択して課金住所を更新します。</span><span class="sxs-lookup"><span data-stu-id="6dc2a-121">Click **Billing profiles** and select a select a billing profile to update the billing address.</span></span>
1. <span data-ttu-id="6dc2a-122">**[プロパティ]** > **[住所の更新]** の順にクリックします。</span><span class="sxs-lookup"><span data-stu-id="6dc2a-122">Click **Properties** > **Update address**.</span></span>
1. <span data-ttu-id="6dc2a-123">新しい住所を入力し、**[保存]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="6dc2a-123">Enter the new address and then click **Save**.</span></span>

<span data-ttu-id="6dc2a-124">**おすすめのドキュメント**</span><span class="sxs-lookup"><span data-stu-id="6dc2a-124">**Recommended documents**</span></span>

<span data-ttu-id="6dc2a-125">[Azure 課金アカウントの連絡先情報を変更する](https://docs.microsoft.com/azure/cost-management-billing/manage/change-azure-account-profile) </span><span class="sxs-lookup"><span data-stu-id="6dc2a-125">[Change contact information for an Azure billing account](https://docs.microsoft.com/azure/cost-management-billing/manage/change-azure-account-profile) </span></span>  
[<span data-ttu-id="6dc2a-126">課金アカウントの設定を更新する</span><span class="sxs-lookup"><span data-stu-id="6dc2a-126">Update billing account settings</span></span>](https://docs.microsoft.com/microsoft-store/update-microsoft-store-for-business-account-settings)  
[<span data-ttu-id="6dc2a-127">Azure での Microsoft 顧客契約の管理者の役割を理解する</span><span class="sxs-lookup"><span data-stu-id="6dc2a-127">Understand Microsoft Customer Agreement administrative roles in Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)