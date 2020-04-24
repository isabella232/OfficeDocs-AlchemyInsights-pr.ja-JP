---
title: メールボックスの自動返信を設定する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 4ffe8d77dad7db5fd5806fe879cf4934e5ca7c4a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2020
ms.locfileid: "43788887"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="18f64-102">ユーザーのメールボックスの自動返信を設定する</span><span class="sxs-lookup"><span data-stu-id="18f64-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="18f64-103">**方法 1**</span><span class="sxs-lookup"><span data-stu-id="18f64-103">**Method 1**</span></span>

1. <span data-ttu-id="18f64-104">Microsoft 365 ポータルにサインインします。</span><span class="sxs-lookup"><span data-stu-id="18f64-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="18f64-105">**[ユーザー]、[アクティブ ユーザー]** (またはこれを共有メールボックスに設定した場合は、**[グループ]、[共有メールボックス]**) の順に移動します。</span><span class="sxs-lookup"><span data-stu-id="18f64-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="18f64-106">Microsoft Exchange メールボックスを持つユーザーを選択します。</span><span class="sxs-lookup"><span data-stu-id="18f64-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="18f64-107">右側のフライアウト メニューで、**[メールの設定]、[自動返信]** の順に移動します (共有メールボックスの場合は、フライアウトで **[自動返信]** をクリックします)。</span><span class="sxs-lookup"><span data-stu-id="18f64-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="18f64-108">**方法 2**</span><span class="sxs-lookup"><span data-stu-id="18f64-108">**Method 2**</span></span>

1. <span data-ttu-id="18f64-109">管理者の資格情報を使用して Microsoft 365 管理ポータルにサインインします。</span><span class="sxs-lookup"><span data-stu-id="18f64-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="18f64-110">**[管理センター]** を展開し、**[Exchange]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="18f64-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="18f64-111">右上隅の画像をクリックし、**[別のユーザー]** をクリックして、変更するユーザーのメールボックスを選択します。</span><span class="sxs-lookup"><span data-stu-id="18f64-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="18f64-112">左側で、**[オプション]** を選択し、**[メールの整理]**、**[自動返信]** の順にクリックします。</span><span class="sxs-lookup"><span data-stu-id="18f64-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="18f64-113">**方法 3**</span><span class="sxs-lookup"><span data-stu-id="18f64-113">**Method 3**</span></span>

<span data-ttu-id="18f64-114">Exchange Online PowerShell で次のコマンドレットを実行します。</span><span class="sxs-lookup"><span data-stu-id="18f64-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="18f64-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="18f64-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="18f64-116">このコマンドレットの詳細については、「[Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="18f64-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
