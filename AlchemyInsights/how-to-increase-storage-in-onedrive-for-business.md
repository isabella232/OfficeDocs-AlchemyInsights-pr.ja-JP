---
title: OneDrive for Business の記憶域を増やす方法
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ceaa6256-a9d9-4fef-a274-d7219365e07f
ms.openlocfilehash: 53eabf6c87dead3b7309c7da1f8a590940127169
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780100"
---
# <a name="how-to-increase-storage-in-onedrive-for-business"></a><span data-ttu-id="07176-102">OneDrive for Business の記憶域を増やす方法</span><span class="sxs-lookup"><span data-stu-id="07176-102">How to increase storage in OneDrive for Business</span></span>

<span data-ttu-id="07176-103">新規および既存の OneDrive ユーザーの既定の記憶域を変更するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="07176-103">To change the default storage for new and existing OneDrive users:</span></span>
  
- <span data-ttu-id="07176-104">[OneDrive 管理センターの [記憶域] ページ](https://admin.onedrive.com/?v=StorageSettings)に移動してから、新しい容量を GB 単位で入力します。</span><span class="sxs-lookup"><span data-stu-id="07176-104">Go to the [Storage page of the OneDrive admin center](https://admin.onedrive.com/?v=StorageSettings), and then enter a new amount in GB.</span></span>

<span data-ttu-id="07176-p101">この記憶域スペースの設定は、特定の記憶域制限を設定していないすべてのユーザーに適用されます。特定のユーザーの記憶域スペースを変更するには、Microsoft PowerShell を使用する必要があります。この方法の詳細については、「[PowerShell を使用してユーザーの OneDrive の容量を変更する](https://go.microsoft.com/fwlink/?linkid=866402)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="07176-p101">This storage space setting applies to all users for whom you haven't set specific storage limits. To change the storage space for specific users, you need to use Microsoft PowerShell. For info on how to do this, see [Change your users' OneDrive storage space using PowerShell](https://go.microsoft.com/fwlink/?linkid=866402).</span></span>

<span data-ttu-id="07176-p102">**メモ**: 無制限の記憶域を含むプランを取得していない可能性があります。各プランに付随する記憶域の詳細については、「[OneDrive for Business サービスの説明](https://go.microsoft.com/fwlink/p/?LinkID=826071)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="07176-p102">**NOTE**: It looks like you don't have a plan that includes unlimited storage. For info about the storage that comes with each plan, see [OneDrive for Business service description](https://go.microsoft.com/fwlink/p/?LinkID=826071).</span></span>
  
<span data-ttu-id="07176-110">OneDrive for Business の記憶域を増やすには、**OneDrive for Business プラン 2** と **Office 365 Enterprise E3** のどちらかのサブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="07176-110">To increase your storage in OneDrive for Business, choose a subscription that includes either **OneDrive for Business Plan 2** or **Office 365 Enterprise E3**.</span></span> 
  
<span data-ttu-id="07176-111">プランを変更するには、Microsoft 365 管理センターで **[課金]** \>**[[製品]](https://go.microsoft.com/fwlink/p/?linkid=842054)** ページの順に移動し、変更するサブスクリプションを選択して **[アップグレード]** タブを選択します。</span><span class="sxs-lookup"><span data-stu-id="07176-111">To change plans, in the Microsoft 365 admin center, go to the **Billing** \> **[Your products](https://go.microsoft.com/fwlink/p/?linkid=842054)** page, select the subscription to change, and then choose the **Upgrade** tab.</span></span>
  
<span data-ttu-id="07176-112">プランの切り替えと OneDrive for Business 記憶域の詳細については、「[別の一般法人向け Microsoft 365 プランに切り替える](https://go.microsoft.com/fwlink/?LinkId=2031117)」と「[OneDrive for Business サービスの説明](https://go.microsoft.com/fwlink/p/?LinkId-2031122)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="07176-112">For more information on switching plans and OneDrive for Business storage, see [Switch to a different Microsoft 365 for business plan](https://go.microsoft.com/fwlink/?LinkId=2031117) and the [OneDrive for Business Service Description](https://go.microsoft.com/fwlink/p/?LinkId-2031122).</span></span>