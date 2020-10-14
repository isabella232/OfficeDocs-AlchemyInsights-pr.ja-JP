---
title: 305 アーカイブ メールボックスのサイズを増やす
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: 6bebc17eafd8615a6ffa95dbdf16f60768204aa7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47778588"
---
# <a name="increase-the-archive-mailbox-size"></a><span data-ttu-id="d94cf-102">アーカイブ メールボックスの容量を増やす</span><span class="sxs-lookup"><span data-stu-id="d94cf-102">Increase the archive mailbox size</span></span>


<span data-ttu-id="d94cf-103">下記の設定の自動チェックを実行する場合は、このページの上部にある [戻る <--] ボタンを選択し、メールをアーカイブメールボックスに移動できないユーザーのメールアドレスを入力します。</span><span class="sxs-lookup"><span data-stu-id="d94cf-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who needs their archive mailbox size increased.</span></span>

<span data-ttu-id="d94cf-104">Microsoft 365 では、ユーザー アカウントに割り当てられているライセンスに基づいて、アーカイブ メールボックスのサイズが[制限](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits)されます。</span><span class="sxs-lookup"><span data-stu-id="d94cf-104">Microsoft 365 [limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) the size of archive mailboxes based on the license that's assigned to the user account.</span></span> <span data-ttu-id="d94cf-105">アーカイブ メールボックスが許可されているサイズの 90% に達すると、ユーザーはメール通知を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="d94cf-105">When the archive mailbox reaches 90% of its allowed size, the user receives an email notification.</span></span> <span data-ttu-id="d94cf-106">アーカイブ メールボックスがサイズの上限に達すると、ユーザーは追加のアイテムをアーカイブ メールボックスに移動することができなくなります。</span><span class="sxs-lookup"><span data-stu-id="d94cf-106">When an archive mailbox reaches its size limit, the user can't move more items to the archive mailbox.</span></span> <span data-ttu-id="d94cf-107">アーカイブ メールボックスがサイズの上限に達しても、Microsoft 365 によりサイズが拡張されることはありません。</span><span class="sxs-lookup"><span data-stu-id="d94cf-107">Microsoft 365 won't increase the size of an archive mailbox once the size limit is reached.</span></span> <span data-ttu-id="d94cf-108">代わりに、ユーザーは次の操作を実行するとアーカイブ メールボックスの領域を開放することができます。</span><span class="sxs-lookup"><span data-stu-id="d94cf-108">Instead, users can take the following actions to free up space in the archive mailbox:</span></span>

- <span data-ttu-id="d94cf-109">Outlook を使用してアイテムを .pst ファイルにエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="d94cf-109">Export the the items to a .pst file using Outlook.</span></span>

- <span data-ttu-id="d94cf-110">アーカイブ メールボックスからアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="d94cf-110">Delete items from the archive mailbox.</span></span>

<span data-ttu-id="d94cf-111">Microsoft 365 では、Office 365 Enterprise E3 および E5 のライセンスで**無制限アーカイブ**が提供されています。</span><span class="sxs-lookup"><span data-stu-id="d94cf-111">Microsoft 365 provides **unlimited archiving** for Office 365 Enterprise E3 and E5 licenses.</span></span> <span data-ttu-id="d94cf-112">管理者は、アーカイブ メールボックスのサイズが最大サイズに達する前にこの機能を有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="d94cf-112">An admin must enable this feature before the archive mailbox reaches its maximum size.</span></span> <span data-ttu-id="d94cf-113">無制限アーカイブが有効になっている場合、アーカイブ メールボックスに空き領域が追加されるまで最大で 30 日かかります。</span><span class="sxs-lookup"><span data-stu-id="d94cf-113">When unlimited archiving is enabled, it can take up to 30 days before free space is added to the archive mailbox.</span></span> <span data-ttu-id="d94cf-114">このため、サイズが拡大される間もユーザーがアーカイブ メールボックスを使用し続けることができるよう、管理者はアーカイブ メールボックスの空き領域を確認することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="d94cf-114">Therefore, we recommend that admins verify the free space in the archive mailbox, which allows the user to continue using the archive mailbox while it expands.</span></span> <span data-ttu-id="d94cf-115">詳細については、「[Microsoft 365 での無制限アーカイブの概要](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving)」と「[Microsoft 365 で無制限アーカイブを有効にする](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d94cf-115">For more information, see [Overview of unlimited archiving in Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving) and [Enable unlimited archiving in Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving).</span></span>

<span data-ttu-id="d94cf-116">Outlook からアーカイブ メールボックスにアクセスする方法の詳細については、「[自動拡張アーカイブ内のアイテムにアクセスするための Outlook の要件](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d94cf-116">For more information on accessing the archive mailbox from Outlook, see [Outlook requirements for accessing items in an auto-expanded archive](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive).</span></span> <span data-ttu-id="d94cf-117">アイテムをアーカイブ メールボックスに自動的に移動するアイテム保持ポリシーを構成する方法については、「[Microsoft 365 組織のメールボックスのアーカイブおよび削除ポリシーを設定する](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d94cf-117">To configure a retention policy that automatically moves items to the archive mailbox, see [Set up an archive and deletion policy for mailboxes in your Microsoft 365 organization](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes).</span></span>

<span data-ttu-id="d94cf-118">**注**: 自動拡張アーカイブは、Exchange 2010 のプライマリ メールボックスではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d94cf-118">**Note**: Auto-expanding archives aren't supported for primary mailboxes on Exchange 2010.</span></span>
