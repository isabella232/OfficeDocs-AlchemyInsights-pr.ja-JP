---
title: 最新の Azure のメールによる請求書
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
- "9003801"
- "6866"
ms.openlocfilehash: 4df8c49880fe638c1659f76edc0905532d091e45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820831"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="dbe7f-102">Azure のメールによる請求書</span><span class="sxs-lookup"><span data-stu-id="dbe7f-102">Email invoicing in Azure</span></span>

<span data-ttu-id="dbe7f-103">メールによる請求書の優先設定を更新するには、課金プロファイルや請求先アカウントで所有者または共同作成者の役割であることが必要です。</span><span class="sxs-lookup"><span data-stu-id="dbe7f-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="dbe7f-104">選択したら、所有者、共同作成者、閲覧者、および請求書管理者ロールを持つすべてのユーザーが、課金プロファイルでメールでの請求書を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="dbe7f-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="dbe7f-105">[Azure portal](https://portal.azure.com/) にサインインします。</span><span class="sxs-lookup"><span data-stu-id="dbe7f-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="dbe7f-106">**コストの管理と課金** で検索します。</span><span class="sxs-lookup"><span data-stu-id="dbe7f-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="dbe7f-107">左側の **[請求書]** を選択し、ページの上部にある **[メールの請求書]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="dbe7f-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="dbe7f-108">複数の課金プロファイルがある場合は、そのうちの 1 つを選択して **[オプトイン]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="dbe7f-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="dbe7f-109">**[更新]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="dbe7f-109">Select **Update**.</span></span>
6. <span data-ttu-id="dbe7f-110">複数の課金プロファイルがある場合は、そのうちの 1 つを選択して **[オプトイン]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="dbe7f-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="dbe7f-111">他のユーザーに表示、ダウンロード、および請求書の支払いのアクセス許可を付与するには、MCA または MPA 課金プロファイルの請求書管理者ロールを割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="dbe7f-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="dbe7f-112">メールで請求書を受け取ることを選択した場合は、ユーザーもメールで請求書を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="dbe7f-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="dbe7f-113">[Azure portal](https://portal.azure.com/) にサインインします。</span><span class="sxs-lookup"><span data-stu-id="dbe7f-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="dbe7f-114">**コストの管理と課金** で検索します。</span><span class="sxs-lookup"><span data-stu-id="dbe7f-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="dbe7f-115">左側の [**課金プロファイル**] を選びます。</span><span class="sxs-lookup"><span data-stu-id="dbe7f-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="dbe7f-116">課金プロファイルの一覧で、請求書管理者ロールを割り当てる課金プロファイルを選びます。</span><span class="sxs-lookup"><span data-stu-id="dbe7f-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="dbe7f-117">左側で **アクセス制御 (IAM)** を選択し、ページの上部にある [**追加**] を選びます。</span><span class="sxs-lookup"><span data-stu-id="dbe7f-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="dbe7f-118">[役割] ドロップダウン リストで、[**請求書管理者**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="dbe7f-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="dbe7f-119">アクセス権を付与するユーザーのメール アドレスを入力します。</span><span class="sxs-lookup"><span data-stu-id="dbe7f-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="dbe7f-120">[**保存**] を選択して、ロールを割り当てます。</span><span class="sxs-lookup"><span data-stu-id="dbe7f-120">Select **Save** to assign the role.</span></span>
