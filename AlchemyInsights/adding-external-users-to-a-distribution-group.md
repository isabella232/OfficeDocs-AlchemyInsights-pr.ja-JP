---
title: 外部ユーザーを配布グループに追加する
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737878"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="e31b7-102">外部ユーザーを配布グループに追加する</span><span class="sxs-lookup"><span data-stu-id="e31b7-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="e31b7-103">外部連絡先を配布グループ (DG) に追加するには、2段階の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="e31b7-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="e31b7-104">外部ユーザーのメール連絡先を作成する:</span><span class="sxs-lookup"><span data-stu-id="e31b7-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="e31b7-105">管理センターで、[**ユーザー** > の[連絡先](https://admin.microsoft.com/adminportal/home#/Contact)] ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="e31b7-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="e31b7-106">[**連絡先の追加**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="e31b7-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="e31b7-107">連絡先の情報を入力し、[**追加**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="e31b7-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="e31b7-108">メール連絡先を DG に追加する:</span><span class="sxs-lookup"><span data-stu-id="e31b7-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="e31b7-109">管理センターで、[**グループ** > [グループ](https://admin.microsoft.com/adminportal/home#/groups)] ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="e31b7-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="e31b7-110">外部ユーザーの追加先となる DG を見つけ、それを選択して [編集] ダイアログを開きます。</span><span class="sxs-lookup"><span data-stu-id="e31b7-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="e31b7-111">[**メンバー** ] タブで、[**すべて表示**] を選択し、メンバーを管理します。</span><span class="sxs-lookup"><span data-stu-id="e31b7-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="e31b7-112">[**メンバーの追加**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="e31b7-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="e31b7-113">前の手順で作成したメール連絡先を選択し、[**保存**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="e31b7-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="e31b7-114">これらの手順を実行した後、外部ユーザーがメールを DG に送信できない、またはメールを受信できない場合は、DG が内部ユーザーからの電子メールのみを許可するように設定されている可能性があります。</span><span class="sxs-lookup"><span data-stu-id="e31b7-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="e31b7-115">この構成を確認して、[ここに記載](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)されている手順に従って修正することができます。</span><span class="sxs-lookup"><span data-stu-id="e31b7-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="e31b7-116">**注:** これらの手順は、グループの種類が "配布グループ" ではなく "Office 365 group" である場合には適用されません。</span><span class="sxs-lookup"><span data-stu-id="e31b7-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="e31b7-117">その場合は、Outlook から直接グループに外部ユーザーを追加することができます。</span><span class="sxs-lookup"><span data-stu-id="e31b7-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="e31b7-118">Office 365 グループゲストの詳細と、外部ゲストの追加手順については、[この記事](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e31b7-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  