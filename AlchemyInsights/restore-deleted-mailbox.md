---
title: 削除済みメールボックスを復元する
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "360"
- "3500005"
search.appverid:
- MOE150
- MED150
- MBS150
ms.assetid: e6112a76-bbb6-4c22-b2e6-690b004d92d4
ms.openlocfilehash: 44b23be5e75a0669821bbeb07b0f064eeef6d021
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666377"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="e28b5-102">削除済みメールボックスを復元する</span><span class="sxs-lookup"><span data-stu-id="e28b5-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="e28b5-103">ユーザーの Exchange Online のライセンスが失われても、そのメールボックスは 30 日間保持され、ユーザーにライセンスを再割り当てすると復元できます。</span><span class="sxs-lookup"><span data-stu-id="e28b5-103">When the user loses its Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
 <span data-ttu-id="e28b5-104">*これは、30 日間に限り有効です。*</span><span class="sxs-lookup"><span data-stu-id="e28b5-104">*This will work only within 30 days.*  In the Admin Portal, go to:</span></span>  
  
1. <span data-ttu-id="e28b5-105">Microsoft 365 管理センターで、**[ユーザー]** \> **[アクティブなユーザー]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="e28b5-105">In the Microsoft 365 admin center, choose Users to go to the Active users page.</span></span> <span data-ttu-id="e28b5-106">該当するユーザーを選択します。</span><span class="sxs-lookup"><span data-stu-id="e28b5-106">UsersActive users. Select the user in question.</span></span>

2. <span data-ttu-id="e28b5-107">**[ライセンスとアプリ]** タブで、Exchange Online ライセンスを割り当て、**[変更の保存]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="e28b5-107">On the **Licenses and Apps** tab, assign the Exchange Online license and select **Save changes**.</span></span>

<span data-ttu-id="e28b5-108">共有メールボックスを復元しようとしている場合も、復元可能な期間は 30 日間です。</span><span class="sxs-lookup"><span data-stu-id="e28b5-108">If you are trying to recover a Shared mailbox, it is also recoverable for 30 days. You can find them under UsersDeleted users. Shared mailboxes do not require a license.</span></span> <span data-ttu-id="e28b5-109">**ユーザー** \> \*\*削除されたユーザー \*\* で確認できます; 共有メールボックスにライセンスは必要ありません。</span><span class="sxs-lookup"><span data-stu-id="e28b5-109">You can find them under **Users** \> **Deleted users**; shared mailboxes do not require a license.</span></span> <span data-ttu-id="e28b5-110">削除したユーザーを復元する必要がある場合は、[「Office 365 でユーザーを復元する」](https://docs.microsoft.com/office365/admin/add-users/restore-user) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e28b5-110">If you realize that you need to restore a deleted user, please see [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user).</span></span>
  