---
title: 305 アーカイブ メールボックスのサイズを増やす
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: f80b2a10ebc17cd98ed1d29b0e6ba3ca01eb1d62
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508813"
---
# <a name="increase-the-archive-mailbox-size"></a><span data-ttu-id="cb812-102">アーカイブ メールボックスの容量を増やす</span><span class="sxs-lookup"><span data-stu-id="cb812-102">Increase the archive mailbox size</span></span>

<span data-ttu-id="cb812-103">Microsoft 365 では、ユーザー アカウントに割り当てられているライセンスに基づいて、アーカイブ メールボックスのサイズが[制限](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits)されます。</span><span class="sxs-lookup"><span data-stu-id="cb812-103">Microsoft 365 [limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) the size of archive mailboxes based on the license that's assigned to the user account.</span></span> <span data-ttu-id="cb812-104">アーカイブ メールボックスが許可されているサイズの 90% に達すると、ユーザーはメール通知を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="cb812-104">When the archive mailbox reaches 90% of its allowed size, the user receives an email notification.</span></span> <span data-ttu-id="cb812-105">アーカイブ メールボックスがサイズの上限に達すると、ユーザーは追加のアイテムをアーカイブ メールボックスに移動することができなくなります。</span><span class="sxs-lookup"><span data-stu-id="cb812-105">When an archive mailbox reaches its size limit, the user can't move more items to the archive mailbox.</span></span> <span data-ttu-id="cb812-106">アーカイブ メールボックスがサイズの上限に達しても、Microsoft 365 によりサイズが拡張されることはありません。</span><span class="sxs-lookup"><span data-stu-id="cb812-106">Microsoft 365 won't increase the size of an archive mailbox once the size limit is reached.</span></span> <span data-ttu-id="cb812-107">代わりに、ユーザーは次の操作を実行するとアーカイブ メールボックスの領域を開放することができます。</span><span class="sxs-lookup"><span data-stu-id="cb812-107">Instead, users can take the following actions to free up space in the archive mailbox:</span></span>

- <span data-ttu-id="cb812-108">Outlook を使用してアイテムを .pst ファイルにエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="cb812-108">Export the the items to a .pst file using Outlook.</span></span>

- <span data-ttu-id="cb812-109">アーカイブ メールボックスからアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="cb812-109">Delete items from the archive mailbox.</span></span>

<span data-ttu-id="cb812-110">Microsoft 365 では、Office 365 Enterprise E3 および E5 のライセンスで**無制限アーカイブ**が提供されています。</span><span class="sxs-lookup"><span data-stu-id="cb812-110">Microsoft 365 provides **unlimited archiving** for Office 365 Enterprise E3 and E5 licenses.</span></span> <span data-ttu-id="cb812-111">管理者は、アーカイブ メールボックスのサイズが最大サイズに達する前にこの機能を有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="cb812-111">An admin must enable this feature before the archive mailbox reaches its maximum size.</span></span> <span data-ttu-id="cb812-112">無制限アーカイブが有効になっている場合、アーカイブ メールボックスに空き領域が追加されるまで最大で 30 日かかります。</span><span class="sxs-lookup"><span data-stu-id="cb812-112">When unlimited archiving is enabled, it can take up to 30 days before free space is added to the archive mailbox.</span></span> <span data-ttu-id="cb812-113">このため、サイズが拡大される間もユーザーがアーカイブ メールボックスを使用し続けることができるよう、管理者はアーカイブ メールボックスの空き領域を確認することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="cb812-113">Therefore, we recommend that admins verify the free space in the archive mailbox, which allows the user to continue using the archive mailbox while it expands.</span></span> <span data-ttu-id="cb812-114">詳細については、「[Microsoft 365 での無制限アーカイブの概要](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving)」と「[Microsoft 365 で無制限アーカイブを有効にする](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cb812-114">For more information, see [Overview of unlimited archiving in Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving) and [Enable unlimited archiving in Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving).</span></span>

<span data-ttu-id="cb812-115">Outlook からアーカイブ メールボックスにアクセスする方法の詳細については、「[自動拡張アーカイブ内のアイテムにアクセスするための Outlook の要件](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cb812-115">For more information on accessing the archive mailbox from Outlook, see [Outlook requirements for accessing items in an auto-expanded archive](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive).</span></span> <span data-ttu-id="cb812-116">アイテムをアーカイブ メールボックスに自動的に移動するアイテム保持ポリシーを構成する方法については、「[Microsoft 365 組織のメールボックスのアーカイブおよび削除ポリシーを設定する](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cb812-116">To configure a retention policy that automatically moves items to the archive mailbox, see [Set up an archive and deletion policy for mailboxes in your Microsoft 365 organization](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes).</span></span>

<span data-ttu-id="cb812-117">**注**: 自動拡張アーカイブは、Exchange 2010 のプライマリ メールボックスではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cb812-117">**Note**: Auto-expanding archives aren't supported for primary mailboxes on Exchange 2010.</span></span>
