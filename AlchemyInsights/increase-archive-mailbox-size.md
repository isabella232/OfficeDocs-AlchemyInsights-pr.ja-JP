---
title: 305アーカイブメールボックスのサイズを増やす
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: a8c16d97040e9396d6cf9bd4a5da671a7da88e13
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/15/2019
ms.locfileid: "36661805"
---
# <a name="increase-the-archive-mailbox-size"></a><span data-ttu-id="2181e-102">アーカイブメールボックスのサイズを増やす</span><span class="sxs-lookup"><span data-stu-id="2181e-102">Increase the archive mailbox size</span></span>

<span data-ttu-id="2181e-103">Office 365 では、ユーザーアカウントに割り当てられているライセンスに基づいて、アーカイブメールボックスのサイズが[制限](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits)されます。</span><span class="sxs-lookup"><span data-stu-id="2181e-103">Office 365 [limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) the size of archive mailboxes based on the license that's assigned to the user account.</span></span> <span data-ttu-id="2181e-104">アーカイブメールボックスが許可されたサイズの90% に達すると、ユーザーはメール通知を受信します。</span><span class="sxs-lookup"><span data-stu-id="2181e-104">When the archive mailbox reaches 90% of its allowed size, the user receives an email notification.</span></span> <span data-ttu-id="2181e-105">アーカイブメールボックスのサイズが制限に達した場合、ユーザーはそれより多くのアイテムをアーカイブメールボックスに移動することはできません。</span><span class="sxs-lookup"><span data-stu-id="2181e-105">When an archive mailbox reaches its size limit, the user can't move more items to the archive mailbox.</span></span> <span data-ttu-id="2181e-106">サイズ制限に達した後、Office 365 はアーカイブメールボックスのサイズを拡大しません。</span><span class="sxs-lookup"><span data-stu-id="2181e-106">Office 365 won't increase the size of an archive mailbox once the size limit is reached.</span></span> <span data-ttu-id="2181e-107">代わりに、ユーザーは次の操作を実行して、アーカイブメールボックス内の空き領域を増やすことができます。</span><span class="sxs-lookup"><span data-stu-id="2181e-107">Instead, users can take the following actions to free up space in the archive mailbox:</span></span>

- <span data-ttu-id="2181e-108">Outlook を使用して、アイテムを .pst ファイルにエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="2181e-108">Export the the items to a .pst file using Outlook.</span></span>

- <span data-ttu-id="2181e-109">アーカイブメールボックスからアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="2181e-109">Delete items from the archive mailbox.</span></span>

<span data-ttu-id="2181e-110">Office 365 では、Office 365 Enterprise E3 および E5 のライセンスに対して**無制限のアーカイブ**が提供されています。</span><span class="sxs-lookup"><span data-stu-id="2181e-110">Office 365 provides **unlimited archiving** for Office 365 Enterprise E3 and E5 licenses.</span></span> <span data-ttu-id="2181e-111">管理者は、アーカイブメールボックスが最大サイズに達する前に、この機能を有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="2181e-111">An admin must enable this feature before the archive mailbox reaches its maximum size.</span></span> <span data-ttu-id="2181e-112">無制限のアーカイブが有効になっている場合は、アーカイブメールボックスに空き領域が追加されるまでに最大で30日かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="2181e-112">When unlimited archiving is enabled, it can take up to 30 days before free space is added to the archive mailbox.</span></span> <span data-ttu-id="2181e-113">そのため、管理者はアーカイブメールボックスの空き領域を確認することをお勧めします。これにより、ユーザーは、拡張中にアーカイブメールボックスを引き続き使用できます。</span><span class="sxs-lookup"><span data-stu-id="2181e-113">Therefore, we recommend that admins verify the free space in the archive mailbox, which allows the user to continue using the archive mailbox while it expands.</span></span> <span data-ttu-id="2181e-114">詳細については、「office [365 での無制限アーカイブの概要](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving)」および「 [office 365 で無制限アーカイブを有効にする](https://docs.microsoft.com/office365/securitycompliance/enable-unlimited-archiving)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2181e-114">For more information, see [Overview of unlimited archiving in Office 365](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving) and [Enable unlimited archiving in Office 365](https://docs.microsoft.com/office365/securitycompliance/enable-unlimited-archiving).</span></span>

<span data-ttu-id="2181e-115">Outlook からアーカイブメールボックスにアクセスする方法の詳細については、「[自動拡張アーカイブのアイテムにアクセスするための outlook 要件](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2181e-115">For more information on accessing the archive mailbox from Outlook, see [Outlook requirements for accessing items in an auto-expanded archive](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive).</span></span> <span data-ttu-id="2181e-116">アイテムをアーカイブメールボックスに自動的に移動するアイテム保持ポリシーを構成するには、「 [Office 365 組織のメールボックスのアーカイブおよび削除ポリシーをセットアップ](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2181e-116">To configure a retention policy that automatically moves items to the archive mailbox, see [Set up an archive and deletion policy for mailboxes in your Office 365 organization](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes).</span></span>

<span data-ttu-id="2181e-117">**注**: 自動拡張アーカイブは、Exchange 2010 のプライマリメールボックスではサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2181e-117">**Note**: Auto-expanding archives aren't supported for primary mailboxes on Exchange 2010.</span></span>
