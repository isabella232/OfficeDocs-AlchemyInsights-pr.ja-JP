---
title: OneDrive 同期クライアントの組織名を変更する
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
- "9003077"
- "5850"
ms.openlocfilehash: ca545ba51e39209f3302acdee1c24048515e2c1b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818329"
---
# <a name="change-the-organization-name-for-the-onedrive-sync-client"></a><span data-ttu-id="362ad-102">OneDrive 同期クライアントの組織名を変更する</span><span class="sxs-lookup"><span data-stu-id="362ad-102">Change the organization name for the OneDrive sync client</span></span>

<span data-ttu-id="362ad-103">OneDrive は、テナント管理者が設定した組織名を使用します。</span><span class="sxs-lookup"><span data-stu-id="362ad-103">OneDrive uses the organization name set by a tenant administrator.</span></span>  <span data-ttu-id="362ad-104">[組織の住所、技術担当者などを変更](https://docs.microsoft.com/microsoft-365/admin/manage/change-address-contact-and-more)できます。</span><span class="sxs-lookup"><span data-stu-id="362ad-104">You can [change your organization's address, technical contact, and more](https://docs.microsoft.com/microsoft-365/admin/manage/change-address-contact-and-more).</span></span> <span data-ttu-id="362ad-105">テナントに対してその変更が実行されると、ユーザーが OneDrive アカウントのリンクを解除して再リンクするまで、OneDrive 同期クライアントは新しい名前を反映しません。</span><span class="sxs-lookup"><span data-stu-id="362ad-105">Once that change is performed for the tenant, the OneDrive sync client will not reflect the new name until users unlink and relink their OneDrive account.</span></span>

<span data-ttu-id="362ad-106">アカウントのリンクを解除するには:</span><span class="sxs-lookup"><span data-stu-id="362ad-106">To unlink the account:</span></span>

1. <span data-ttu-id="362ad-107">タスクバーの右端にある青い OneDrive クラウド アイコンを選択し、**[その他]、[設定]、[アカウント]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="362ad-107">Select the blue OneDrive cloud icon at the far right of the taskbar, then select  **More > Settings > Account**.</span></span>
2. <span data-ttu-id="362ad-108">リンクを解除するア​​カウントを見つけて、[**この PC のリンク解除**] を選択し、次に [**アカウントのリンク解除**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="362ad-108">Find the account you want to unlink and select  **Unlink this PC**, and then  **Unlink account**.</span></span>

<span data-ttu-id="362ad-109">アカウントを再リンクするには、[設定] の [**アカウント**] タブから [**アカウントを追加**] を選択し、OneDrive に再度サインインします。</span><span class="sxs-lookup"><span data-stu-id="362ad-109">To relink the account, select  **Add an account** from the  **Account** tab in Settings, and sign back into OneDrive.</span></span>