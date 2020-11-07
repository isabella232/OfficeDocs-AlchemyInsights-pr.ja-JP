---
title: OneDrive for Business の記憶域を増やす方法
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ceaa6256-a9d9-4fef-a274-d7219365e07f
ms.openlocfilehash: 676b17d47ee5071ed45e8d6022eaa82b51fc4d51
ms.sourcegitcommit: ad2d185aa9e08c27c4a1c4803b679cc4e6305703
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/16/2020
ms.locfileid: "48489024"
---
# <a name="how-to-increase-storage-in-onedrive-for-business"></a><span data-ttu-id="b32da-102">OneDrive for Business の記憶域を増やす方法</span><span class="sxs-lookup"><span data-stu-id="b32da-102">How to increase storage in OneDrive for Business</span></span>

<span data-ttu-id="b32da-103">新規および既存の OneDrive ユーザーの既定の記憶域を変更するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="b32da-103">To change the default storage for new and existing OneDrive users:</span></span>
  
- <span data-ttu-id="b32da-104">[OneDrive 管理センターの [記憶域] ページ](https://admin.onedrive.com/?v=StorageSettings)に移動してから、新しい容量を GB 単位で入力し、 **[保存]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="b32da-104">Go to the [Storage page of the OneDrive admin center](https://admin.onedrive.com/?v=StorageSettings), enter a new amount in GB, then select **Save**.</span></span>

<span data-ttu-id="b32da-p101">この記憶域スペースの設定は、特定の記憶域制限を設定していないすべてのユーザーに適用されます。特定のユーザーの記憶域スペースを変更するには、Microsoft PowerShell を使用します。この方法の詳細については、「[PowerShell を使用してユーザーの OneDrive の容量を変更する](https://docs.microsoft.com/onedrive/change-user-storage)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b32da-p101">This storage space setting applies to all users for whom you haven't set specific storage limits. To change the storage space for specific users, use Microsoft PowerShell. For info on how to do this, see [Change your users' OneDrive storage space using PowerShell](https://docs.microsoft.com/onedrive/change-user-storage).</span></span>

<span data-ttu-id="b32da-p102">**メモ** : 無制限の記憶域を含むプランを取得していない可能性があります。各プランに付随する記憶域の詳細については、「 [OneDrive for Business サービスの説明](https://docs.microsoft.com/office365/servicedescriptions/onedrive-for-business-service-description)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b32da-p102">**NOTE** : It looks like you don't have a plan that includes unlimited storage. For info about the storage that comes with each plan, see [OneDrive for Business service description](https://docs.microsoft.com/office365/servicedescriptions/onedrive-for-business-service-description).</span></span>
  
<span data-ttu-id="b32da-110">OneDrive for Business の記憶域を増やすには、 **OneDrive for Business プラン 2** または **Office 365 E3** のどちらかのサブスクリプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="b32da-110">To increase your storage in OneDrive for Business, choose a subscription that includes either **OneDrive for Business Plan 2** or **Office 365 E3**.</span></span>
  
<span data-ttu-id="b32da-111">プランを変更するには、管理センターで **[課金]** \> [[製品]](https://go.microsoft.com/fwlink/p/?linkid=842054) ページの順に移動し、変更するサブスクリプションを選択して **組織向けの推奨アップグレードを表示する** を選択します。</span><span class="sxs-lookup"><span data-stu-id="b32da-111">To change plans, in the admin center, go to the **Billing** \> [Your products](https://go.microsoft.com/fwlink/p/?linkid=842054) page, select the subscription to change, then choose **View upgrades recommended for your org**.</span></span>
  
<span data-ttu-id="b32da-112">プランの切り替えと OneDrive for Business 記憶域の詳細については、「[別のプランにアップグレードする](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan)」 と 「[OneDrive for Business サービスの説明](https://docs.microsoft.com/office365/servicedescriptions/onedrive-for-business-service-description)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b32da-112">For more information on changing plans and OneDrive for Business storage, see [Upgrade to a different plan](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan) and the [OneDrive for Business Service Description](https://docs.microsoft.com/office365/servicedescriptions/onedrive-for-business-service-description).</span></span>