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
ms.openlocfilehash: 14d2c9b1fe6764f5cd3a5a968586a19a03b62694
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/10/2021
ms.locfileid: "50641523"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="8f0a3-102">削除済みメールボックスを復元する</span><span class="sxs-lookup"><span data-stu-id="8f0a3-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="8f0a3-103">ユーザーの Exchange Online のライセンスが失われても、そのメールボックスは 30 日間保持され、ユーザーにライセンスを再割り当てすると復元できます。</span><span class="sxs-lookup"><span data-stu-id="8f0a3-103">When a user loses an Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
1. <span data-ttu-id="8f0a3-104">Microsoft 365 管理センターで、**[ユーザー]** \> **[アクティブなユーザー]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="8f0a3-104">In the Microsoft 365 admin center, go to the **Users** \> **Active users** page.</span></span> <span data-ttu-id="8f0a3-105">該当するユーザーを選択します。</span><span class="sxs-lookup"><span data-stu-id="8f0a3-105">Select the user in question.</span></span>

2. <span data-ttu-id="8f0a3-106">**[ライセンスとアプリ]** タブで、Exchange Online ライセンスを割り当て、**[変更の保存]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8f0a3-106">On the **Licenses and Apps** tab, assign the Exchange Online license and select **Save changes**.</span></span>

<span data-ttu-id="8f0a3-107">削除された共有メールボックスまたはユーザーを復元しようとしている場合も、復元可能な期間は 30 日間です。</span><span class="sxs-lookup"><span data-stu-id="8f0a3-107">If you are trying to recover a shared mailbox or a user that was deleted, it is also recoverable for 30 days.</span></span> <span data-ttu-id="8f0a3-108">**[ユーザー]** \> **[削除済みのユーザー]** の順に選択して確認できます。共有メールボックスにライセンスは必要ありません。</span><span class="sxs-lookup"><span data-stu-id="8f0a3-108">You can find them under **Users** \> **Deleted users**; shared mailboxes do not require a license.</span></span> <span data-ttu-id="8f0a3-109">「[ユーザーを復元する](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8f0a3-109">Please see [Restore a user](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="8f0a3-110">ユーザーのメールボックスからのメールの復元は、管理者が[新しい Exchange 管理センター](https://techcommunity.microsoft.com/t5/exchange-team-blog/a-new-recoverableitems-experience-comes-to-exchange-online/ba-p/1505353)に移動することにより行うことができます。</span><span class="sxs-lookup"><span data-stu-id="8f0a3-110">Recovery of email from user's mailbox can be done by admins by going to the [new Exchange Admin Center](https://techcommunity.microsoft.com/t5/exchange-team-blog/a-new-recoverableitems-experience-comes-to-exchange-online/ba-p/1505353).</span></span>

<span data-ttu-id="8f0a3-111">最後に、非アクティブなメールボックスを復元する場合は、[こちらの手順に従ってください](https://docs.microsoft.com/microsoft-365/compliance/recover-an-inactive-mailbox)。</span><span class="sxs-lookup"><span data-stu-id="8f0a3-111">Finally, if you are trying to recover an Inactive mailbox, [follow the instructions here](https://docs.microsoft.com/microsoft-365/compliance/recover-an-inactive-mailbox).</span></span>
  
