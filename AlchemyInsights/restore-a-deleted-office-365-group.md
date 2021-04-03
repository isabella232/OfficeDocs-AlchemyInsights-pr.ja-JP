---
title: 削除された Microsoft 365 グループを復元する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505691"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="f5f00-102">削除された Microsoft 365 グループを復元する</span><span class="sxs-lookup"><span data-stu-id="f5f00-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="f5f00-103">削除された Microsoft 365 グループまたは Microsoft Teams は、削除から 30 日以内なら復元できます。</span><span class="sxs-lookup"><span data-stu-id="f5f00-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="f5f00-104">Microsoft 365 管理センターにログインし、削除したグループとチームを一覧表示します。 [「Microsoft 365 管理センター」](https://aka.ms/RestoreDeletedGroup)に移動します。</span><span class="sxs-lookup"><span data-stu-id="f5f00-104">To login to Microsoft 365 admin center and list the deleted groups and teams, go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup).</span></span>

    <span data-ttu-id="f5f00-105">**注:** テナントの管理者またはグループ管理者の役割に割り当てられているアカウントを使用してログインします。</span><span class="sxs-lookup"><span data-stu-id="f5f00-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="f5f00-106">復元する削除済み Microsoft 365 グループ/Teams を選択し、**[グループの復元]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="f5f00-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="f5f00-107">SMTP アドレスが競合するためにグループを復元できない場合は、次のコマンドを使用して競合の原因となっているオブジェクトを探し、SMTP アドレスを削除します。</span><span class="sxs-lookup"><span data-stu-id="f5f00-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="f5f00-108">**注:** グループとそのすべてのデータが完全に復元されるまで 24 時間ほどかかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="f5f00-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="f5f00-109">詳細な情報、または PowerShell を使用したグループの復元方法については、「[削除された Microsoft 365 グループを復元する](https://go.microsoft.com/fwlink/?linkid=867802)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f5f00-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>