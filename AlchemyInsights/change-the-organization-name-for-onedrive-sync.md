---
title: OneDrive 同期クライアントの組織名を変更する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003077"
- "5850"
ms.openlocfilehash: 8e474276633bba2895338fd0c0a5903df1ddf637
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756720"
---
# <a name="change-the-organization-name-for-the-onedrive-sync-client"></a><span data-ttu-id="8a401-102">OneDrive 同期クライアントの組織名を変更する</span><span class="sxs-lookup"><span data-stu-id="8a401-102">Change the organization name for the OneDrive sync client</span></span>

<span data-ttu-id="8a401-103">OneDrive は、テナント管理者が設定した組織名を使用します。</span><span class="sxs-lookup"><span data-stu-id="8a401-103">OneDrive uses the organization name set by a tenant administrator.</span></span>  <span data-ttu-id="8a401-104">[組織の住所、技術担当者などを変更](https://docs.microsoft.com/microsoft-365/admin/manage/change-address-contact-and-more)できます。</span><span class="sxs-lookup"><span data-stu-id="8a401-104">You can [change your organization's address, technical contact, and more](https://docs.microsoft.com/microsoft-365/admin/manage/change-address-contact-and-more).</span></span> <span data-ttu-id="8a401-105">テナントに対してその変更が実行されると、ユーザーが OneDrive アカウントのリンクを解除して再リンクするまで、OneDrive 同期クライアントは新しい名前を反映しません。</span><span class="sxs-lookup"><span data-stu-id="8a401-105">Once that change is performed for the tenant, the OneDrive sync client will not reflect the new name until users unlink and relink their OneDrive account.</span></span>

<span data-ttu-id="8a401-106">アカウントのリンクを解除するには:</span><span class="sxs-lookup"><span data-stu-id="8a401-106">To unlink the account:</span></span>

1. <span data-ttu-id="8a401-107">タスクバーの右端にある青い OneDrive クラウド アイコンを選択し、**[その他]、[設定]、[アカウント]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="8a401-107">Select the blue OneDrive cloud icon at the far right of the taskbar, then select  **More > Settings > Account**.</span></span>
2. <span data-ttu-id="8a401-108">リンクを解除するア​​カウントを見つけて、[**この PC のリンク解除**] を選択し、次に [**アカウントのリンク解除**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="8a401-108">Find the account you want to unlink and select  **Unlink this PC**, and then  **Unlink account**.</span></span>

<span data-ttu-id="8a401-109">アカウントを再リンクするには、[設定] の [**アカウント**] タブから [**アカウントを追加**] を選択し、OneDrive に再度サインインします。</span><span class="sxs-lookup"><span data-stu-id="8a401-109">To relink the account, select  **Add an account** from the  **Account** tab in Settings, and sign back into OneDrive.</span></span>