---
title: 条件付きアクセスの監視
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 06307b57475e8828e6d4e5e01625d5100576f12b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28298299"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="84f5d-102">条件付きアクセスの監視</span><span class="sxs-lookup"><span data-stu-id="84f5d-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="84f5d-p101">条件付きアクセスの対象となるユーザー組織のアクセス要件を満たしていない場合は、メールによる通知が表示されます。を解決するのには、次の解決策の 1 つ以上お勧めします。</span><span class="sxs-lookup"><span data-stu-id="84f5d-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="84f5d-p102">デバイスが登録すると見なされます場合は、会社のポータル アプリケーションに移動し、企業ポータルに表示されたことを確認するユーザーを案内します。しない場合、ユーザーがデバイスを登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="84f5d-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="84f5d-p103">Azure ポータルに移動**Intune\>デバイス対応**です。**モニター** ] の下には、**準拠のデバイス**をクリックします。ユーザーのデバイスに準拠としてマークされていることを確認するのには、デバイスのコンプライアンス レポートを表示します。</span><span class="sxs-lookup"><span data-stu-id="84f5d-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="84f5d-p104">Azure ポータルに移動**Intune\>デバイス対応**です。[**管理**] で [**ポリシー**] をクリックします。コンプライアンス ・ ポリシーの一覧で、プロファイルが、ユーザーのデバイスに割り当てられていることを確認します。プロファイルが割り当てられていない場合 Intune はデバイスのコンプライアンスのステータスを確認できません。</span><span class="sxs-lookup"><span data-stu-id="84f5d-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="84f5d-114">ユーザーの条件付きアクセスの割り当てを編集します。</span><span class="sxs-lookup"><span data-stu-id="84f5d-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="84f5d-115">Azure ポータルに移動**Intune\>条件付きアクセス\>ポリシー**</span><span class="sxs-lookup"><span data-stu-id="84f5d-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="84f5d-116">リストからポリシーを選択します。</span><span class="sxs-lookup"><span data-stu-id="84f5d-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="84f5d-117">[**ユーザーとグループ**</span><span class="sxs-lookup"><span data-stu-id="84f5d-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="84f5d-p105">他のユーザーに特定のポリシーをターゲットに**含める**] ボックスの一覧に追加します。ポリシーから人が省略されていることを確認するには、**除外**リストに追加します。</span><span class="sxs-lookup"><span data-stu-id="84f5d-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="84f5d-120">参照:[デバイスの条件付きのアクセスを監視する方法](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="84f5d-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span></span>
  

