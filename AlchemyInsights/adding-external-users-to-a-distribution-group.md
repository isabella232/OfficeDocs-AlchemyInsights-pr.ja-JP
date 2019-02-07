---
title: 外部ユーザーを配布グループに追加する場合
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 8/22/2017
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 5911d57786dfc512eade1c74831d4260e85b8a1c
ms.sourcegitcommit: 5dee2fcb492bd922092a6de8045a95febe57b97e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/06/2019
ms.locfileid: "29758097"
---
# <a name="adding-external-users-to-a-distribution-group"></a><span data-ttu-id="4d442-102">外部ユーザーを配布グループに追加する場合</span><span class="sxs-lookup"><span data-stu-id="4d442-102">Adding external users to a Distribution Group?</span></span>

<span data-ttu-id="4d442-103">外部の連絡先を配布グループ (DG) に追加する作業は次の 2 段階プロセスになっています。</span><span class="sxs-lookup"><span data-stu-id="4d442-103">Adding an external contact to a Distribution Group (DG) is a 2-step process:</span></span>
  
1. <span data-ttu-id="4d442-104">外部ユーザーのメール連絡先を作成する:</span><span class="sxs-lookup"><span data-stu-id="4d442-104">Create a Mail Contact for the external user:</span></span>
    
1. <span data-ttu-id="4d442-105">[ここ](https://admin.microsoft.com/adminportal/home#/Contact)をクリックし、管理ポータルの連絡先編集ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="4d442-105">Click [here](https://admin.microsoft.com/adminportal/home#/Contact) to navigate to the Contact edit page in the Admin portal.</span></span> 
    
2. <span data-ttu-id="4d442-106">[**連絡先の追加**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="4d442-106">Click on **Add a Contact**.</span></span>
    
3. <span data-ttu-id="4d442-107">連絡先の情報を入力し、[**保存**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="4d442-107">Type the information for your contact and click **Save**.</span></span>
    
2. <span data-ttu-id="4d442-108">メール連絡先を DG に追加する:</span><span class="sxs-lookup"><span data-stu-id="4d442-108">Add the Mail Contact to your DG:</span></span>
    
1. <span data-ttu-id="4d442-109">[ここ](https://admin.microsoft.com/adminportal/home#/groups)をクリックし、グループ ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="4d442-109">Click [here](https://admin.microsoft.com/adminportal/home#/groups) to navigate to the Groups page.</span></span> 
    
2. <span data-ttu-id="4d442-110">外部ユーザーを追加する DG を見つけたらそれをクリックし、編集ダイアログを開きます。</span><span class="sxs-lookup"><span data-stu-id="4d442-110">Find the DG you want to add the external user to, and click on it to open the edit dialog.</span></span>
    
3. <span data-ttu-id="4d442-111">[**メンバー**] 一覧の [**編集**] ボタンをクリックします。</span><span class="sxs-lookup"><span data-stu-id="4d442-111">Click on the **Edit** button in the **Members** list.</span></span> 
    
4. <span data-ttu-id="4d442-112">[**メンバーの追加**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="4d442-112">Click on **Add Members**.</span></span>
    
5. <span data-ttu-id="4d442-113">前の手順で作成したメール連絡先を選択し、[**保存**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="4d442-113">Select the Mail Contact you created on the previous step and click **Save**.</span></span>
    
<span data-ttu-id="4d442-p101">以上の手順に従っても外部ユーザーが DG にメールを送信できないか、DG からメールを受信できない場合、内部ユーザーからのメールのみがその DG に許可されている可能性があります。[こちら](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx)の操作方法に従うことでこの構成を確認し、修正できます。</span><span class="sxs-lookup"><span data-stu-id="4d442-p101">If even after following these steps your external users can't send emails to the DG or don't receive emails from it, it can be that the DG is marked to only allow emails from internal users. You can check this configuration and fix it following the directions [here](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx)</span></span>
  
 <span data-ttu-id="4d442-p102">**注:** グループの種類が "配布グループ" ではなく "Office 365 グループ" の場合、これらの操作方法は適用されません。その場合、外部ユーザーは Outlook または Outlook on the web からグループに直接追加できます。O365 グループ ゲストに関する詳しい説明と外部ゲストの追加方法については、[こちらの記事](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)でご確認いただけます。</span><span class="sxs-lookup"><span data-stu-id="4d442-p102">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group." If that is the case, you can add the external user directly to the group from Outlook or Outlook on the Web. Detailed explanation on O365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  

