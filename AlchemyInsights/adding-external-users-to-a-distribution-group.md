---
title: 外部ユーザーを配布グループに追加する場合
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737878"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="27cb4-102">外部ユーザーを配布グループに追加する場合</span><span class="sxs-lookup"><span data-stu-id="27cb4-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="27cb4-103">外部の連絡先を配布グループ (DG) に追加する作業は次の 2 段階プロセスになっています。</span><span class="sxs-lookup"><span data-stu-id="27cb4-103">Adding an external contact to a Distribution Group (DG) is a 2-step process:</span></span>
  
1. <span data-ttu-id="27cb4-104">外部ユーザーのメール連絡先を作成する:</span><span class="sxs-lookup"><span data-stu-id="27cb4-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="27cb4-105">管理センターで、[**ユーザー**]  >  [[連絡先](https://admin.microsoft.com/adminportal/home#/Contact)] ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="27cb4-105">In the admin center, go to the **Billing**  >  [Subscriptions](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="27cb4-106">[**連絡先を追加する**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="27cb4-106">Select **Add a site**.</span></span>
    
    3. <span data-ttu-id="27cb4-107">連絡先の情報を入力し、[**保存**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="27cb4-107">Type the information for your contact and click **Save**.</span></span>
    
2. <span data-ttu-id="27cb4-108">メール連絡先を DG に追加する:</span><span class="sxs-lookup"><span data-stu-id="27cb4-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="27cb4-109">管理センターで、[**グループ**]  >  [[グループ](https://admin.microsoft.com/adminportal/home#/groups)] ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="27cb4-109">In the admin center, go to the **Groups**  >  [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="27cb4-110">外部ユーザーを追加する DG を見つけたらそれを選択し、編集ダイアログを開きます。</span><span class="sxs-lookup"><span data-stu-id="27cb4-110">Find the DG you want to add the external user to, and click on it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="27cb4-111">[**メンバー**] タブで [**すべてのメンバーの表示と管理**] を選択します。 </span><span class="sxs-lookup"><span data-stu-id="27cb4-111">Select the group, and then on the Members tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="27cb4-112">[**メンバーを追加する**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="27cb4-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="27cb4-113">前の手順で作成したメール連絡先を選択し、[**保存**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="27cb4-113">Select the Mail Contact you created on the previous step and click **Save**.</span></span>
    
<span data-ttu-id="27cb4-114">これらの手順を実行した後に、外部ユーザーと DG の間でメールの送受信ができない場合は、内部ユーザーからのメールのみが許可されるように DG にマークされている可能性があります。</span><span class="sxs-lookup"><span data-stu-id="27cb4-114">If even after following these steps your external users can't send emails to the DG or don't receive emails from it, it can be that the DG is marked to only allow emails from internal users. You can check this configuration and fix it following the directions here</span></span> <span data-ttu-id="27cb4-115">[こちら](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)の指示に従ってこの構成の確認と修正を行えます。</span><span class="sxs-lookup"><span data-stu-id="27cb4-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="27cb4-116">**注:** グループの種類が "配布グループ" ではなく "Office 365 グループ" の場合、これらの手順は適用されません。</span><span class="sxs-lookup"><span data-stu-id="27cb4-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="27cb4-117">その場合は、Outlook からグループに外部ユーザーを直接追加できます。</span><span class="sxs-lookup"><span data-stu-id="27cb4-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="27cb4-118">Office 365 グループ ゲストに関する詳細情報および外部ゲストを追加する手順については、[この記事](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="27cb4-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  