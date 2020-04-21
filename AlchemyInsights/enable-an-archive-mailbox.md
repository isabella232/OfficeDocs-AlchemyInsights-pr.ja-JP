---
title: アーカイブ メールボックスの有効化
ms.author: markjjo
author: markjjo
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "307"
- "3100008"
ms.assetid: e1a5fab7-d3a5-4d4c-8ee2-0edf4ec9b76b
ms.openlocfilehash: da1f12678dd1a508a24f02e73acb6d599eaff628
ms.sourcegitcommit: 940169c0edf638b5086d70cc275049f01dcff3cf
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2020
ms.locfileid: "43132616"
---
# <a name="enable-an-archive-mailbox"></a><span data-ttu-id="e2b43-102">アーカイブ メールボックスの有効化</span><span class="sxs-lookup"><span data-stu-id="e2b43-102">Enable an archive mailbox</span></span>

<span data-ttu-id="e2b43-103">Office 365 のアーカイブ メールボックス (*オンライン アーカイブ*または*インプレース アーカイブ*とも呼ばれます) は、追加のメール ストレージをユーザーに提供します。</span><span class="sxs-lookup"><span data-stu-id="e2b43-103">Archive mailboxes in Office 365 (also called *Online Archives* or *In-Place Archives*) provide users with additional email storage.</span></span> <span data-ttu-id="e2b43-104">ユーザーは、アイテムをアーカイブ メールボックスに移動したり、コピーしたりできます。管理者は、アイテムを自動的にアーカイブ メールボックスに移動させることができる、アーカイブ ポリシーを作成できます。</span><span class="sxs-lookup"><span data-stu-id="e2b43-104">Users can move or copy items to their archive mailbox, and admins can create an archive policy that automatically moves items to archive mailboxes.</span></span>
  
<span data-ttu-id="e2b43-105">アーカイブ メールボックスを作成する方法は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="e2b43-105">Here's how to create an archive mailbox:</span></span>
  
1. <span data-ttu-id="e2b43-106">[https://protection.office.com](https://protection.office.com) に移動します。</span><span class="sxs-lookup"><span data-stu-id="e2b43-106">Go to [https://protection.office.com](https://protection.office.com).</span></span>

2. <span data-ttu-id="e2b43-107">管理者アカウントを使って Office 365 にサインインします。</span><span class="sxs-lookup"><span data-stu-id="e2b43-107">Sign in to Office 365 using your admin account.</span></span>

3. <span data-ttu-id="e2b43-108">セキュリティ/コンプライアンス センター&amp;の左のウィンドウで、**[情報ガバナンス]** \> **[アーカイブ]** の順にクリックします。</span><span class="sxs-lookup"><span data-stu-id="e2b43-108">In the left pane of the Security &amp; Compliance Center, select **Information governance** \> **Archive**.</span></span>

4. <span data-ttu-id="e2b43-109">アーカイブ メールボックスを有効にするユーザーを選択します。</span><span class="sxs-lookup"><span data-stu-id="e2b43-109">Select the user whose archive mailbox you want to enable.</span></span>

5. <span data-ttu-id="e2b43-110">右の詳細ウィンドウで [**有効**] をクリックし、警告メッセージで [**はい**] をクリックしてアーカイブ メールボックスを有効にします。</span><span class="sxs-lookup"><span data-stu-id="e2b43-110">In the details pane on the right, click **Enable** and then click **Yes** in the warning message to enable the archive mailbox.</span></span>

<span data-ttu-id="e2b43-111">アーカイブ メールボックスを一括で有効にするには、(**Shift** キーまたは **Ctrl** キーを使用して) 複数のユーザーを選択し、詳細ウィンドウで [**有効**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="e2b43-111">You can also bulk-enable archive mailboxes by selecting multiple users (using the **Shift** or **Ctrl** keys) and then clicking **Enable** in the details pane.</span></span>
  
### <a name="shared-mailboxes"></a><span data-ttu-id="e2b43-112">共有メールボックス</span><span class="sxs-lookup"><span data-stu-id="e2b43-112">Shared mailboxes</span></span>

<span data-ttu-id="e2b43-113">共有メールボックスのアーカイブを有効にするには、Exchange Online プラン 2 のライセンス、または Exchange Online Archiving のライセンスの付いた Exchange Online プラン 1 のライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="e2b43-113">To enable the archive for a shared mailbox, an Exchange Online Plan 2 license or an Exchange Online Plan 1 license with an Exchange Online Archiving license is required.</span></span>  

<span data-ttu-id="e2b43-114">共有メールボックスのアーカイブを有効にするには、次の操作を行います。</span><span class="sxs-lookup"><span data-stu-id="e2b43-114">To enable the archive for a shared mailbox:</span></span>

1. <span data-ttu-id="e2b43-115">[Exchange 管理センター](https://outlook.office365.com/ecp) に移動し、管理者アカウントを使用してサインインします。</span><span class="sxs-lookup"><span data-stu-id="e2b43-115">Go to the [Exchange admin center](https://outlook.office365.com/ecp) and sign in using your admin account.</span></span>

2. <span data-ttu-id="e2b43-116">**[受信者]** > **[共有]** の順に移動します。</span><span class="sxs-lookup"><span data-stu-id="e2b43-116">Go to **Recipients** > **Shared**.</span></span>

3. <span data-ttu-id="e2b43-117">共有メールボックスを選択します。</span><span class="sxs-lookup"><span data-stu-id="e2b43-117">Select the shared mailbox.</span></span>

4. <span data-ttu-id="e2b43-118">右の詳細ウィンドウの **[インプレース アーカイブ]** で **[有効]** をクリックし、次に **[はい]** をクリックしてアーカイブ メールボックスを有効にします。</span><span class="sxs-lookup"><span data-stu-id="e2b43-118">In the details pane on the right, under **In-Place Archive**, click **Enable**, and then click **Yes** to enable the archive mailbox.</span></span>

<span data-ttu-id="e2b43-119">詳細については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e2b43-119">For more information, see:</span></span>
  
- [<span data-ttu-id="e2b43-120">Office 365 でアーカイブ メールボックスを有効にする</span><span class="sxs-lookup"><span data-stu-id="e2b43-120">Enable archive mailboxes in Office 365</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes)

- [<span data-ttu-id="e2b43-121">Office 365 のアーカイブと削除ポリシーを設定する</span><span class="sxs-lookup"><span data-stu-id="e2b43-121">Set up an archive and deletion policy in Office 365</span></span>](https://docs.microsoft.com//office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)
