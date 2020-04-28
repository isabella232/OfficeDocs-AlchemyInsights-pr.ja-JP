---
title: 条件付きアクセスを監視する
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713723"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="527a9-102">Exchange の条件付きアクセスを監視する</span><span class="sxs-lookup"><span data-stu-id="527a9-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="527a9-p101">条件付きアクセスで対象となるユーザーは、組織のアクセス要件を満たしていない場合には通知電子メールを受信します。この状態を解消するには、以下の 1 つ以上の解決策をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="527a9-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="527a9-p102">そのデバイスが登録されていると推測される場合、ポータル サイト アプリに移動して、ポータル サイトに表示されていることを確認するようユーザーに勧めます。表示されない場合、ユーザーはそのデバイスを登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="527a9-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="527a9-p103">Azure Portal で **[Intune] \> [デバイスのポリシー準拠]** と移動します。**[モニター]** で **[デバイスのポリシー準拠]** をクリックします。デバイスのポリシー準拠レポートを表示して、ユーザーのデバイスがポリシー準拠と示されているかどうか確認します。</span><span class="sxs-lookup"><span data-stu-id="527a9-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="527a9-p104">Azure Portal で **[Intune] \> [デバイスのポリシー準拠]** と移動します。**[管理]** で **[ポリシー]** をクリックします。ポリシー準拠ポリシーの一覧で、ユーザーのデバイスにプロファイルが割り当てられていることを確認します。プロファイルが割り当てられていない場合、Intune はデバイスのポリシー準拠状態を確認できません。</span><span class="sxs-lookup"><span data-stu-id="527a9-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="527a9-114">ユーザーの条件付きアクセス割り当てを編集します。</span><span class="sxs-lookup"><span data-stu-id="527a9-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="527a9-115">Azure Portal で、**[Intune] \> [条件付きアクセス] \> [ポリシー]** と移動します。</span><span class="sxs-lookup"><span data-stu-id="527a9-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="527a9-116">一覧からポリシーを選択します。</span><span class="sxs-lookup"><span data-stu-id="527a9-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="527a9-117">**[ユーザーとグループ]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="527a9-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="527a9-p105">特定のユーザーに対して特定のポリシーを対象とするには、**[必要]** リストに追加します。対象ポリシーから特定のユーザーを除外するには、**[必要なし]** リストに追加します。</span><span class="sxs-lookup"><span data-stu-id="527a9-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="527a9-120">参照資料: [条件付きアクセス デバイスを監視する方法](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="527a9-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

