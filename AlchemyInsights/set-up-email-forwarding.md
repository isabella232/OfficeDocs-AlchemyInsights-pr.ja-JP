---
title: メールの転送をセットアップする
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "20"
- "1200004"
ms.assetid: 15abf81d-5c5d-49da-ac81-1b4daa1809f6
ms.openlocfilehash: 21b967a54e29fc7af85837a38f1efe24525a1f75
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/13/2021
ms.locfileid: "49847605"
---
# <a name="check-the-email-forwarding-settings-for-a-mailbox"></a><span data-ttu-id="ef9dd-102">メールボックスのメールの転送設定を確認する</span><span class="sxs-lookup"><span data-stu-id="ef9dd-102">Check the email forwarding settings for a mailbox</span></span>

<span data-ttu-id="ef9dd-103">まず、テナント レベルでメールの転送を有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="ef9dd-103">Firstly, email forwarding has to be enabled on the tenant level.</span></span> <span data-ttu-id="ef9dd-104">メールの転送をメールボックスに設定しても動作しない場合は、 [「Microsoft 365 での外部メールの自動転送を制御](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding?view=o365-worldwide)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ef9dd-104">If you have set up email forwarding on a mailbox, but it is not working, please see [Control automatic external email forwarding in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding?view=o365-worldwide).</span></span>

<span data-ttu-id="ef9dd-105">メールボックスでメール転送の設定は簡単に確認できます。</span><span class="sxs-lookup"><span data-stu-id="ef9dd-105">It's easy to verify the email forwarding settings on a mailbox!</span></span> <span data-ttu-id="ef9dd-106">次の手順を実行するだけです。</span><span class="sxs-lookup"><span data-stu-id="ef9dd-106">Just follow these steps.</span></span>
  
> <span data-ttu-id="ef9dd-p103">ユーザー メールボックスの場合は、[**ユーザー**] \> [**アクティブなユーザー**] に移動して、転送するメールボックスのユーザーを選択します。[**メール**] タブで、[**メールの転送を管理する**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="ef9dd-p103">If this is a user mailbox, go to **Users** \> **Active users** and select the user whose mailbox you're forwarding. On the **Mail** tab, select **Manage email forwarding**.</span></span>

> <span data-ttu-id="ef9dd-p104">共有メールボックスの場合は、[**グループ**] \> [**共有メールボックス**] に移動して、転送する共有メールボックスを選択します。メールの転送の [**編集**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="ef9dd-p104">If this is a shared mailbox, go to **Groups** \> **Shared mailboxes** and select the shared mailbox you're forwarding. Select **Edit** for email forwarding.</span></span>

<span data-ttu-id="ef9dd-111">詳細については、「[Microsoft 365 でメール転送を構成する](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ef9dd-111">For more information, see [Configure email forwarding in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>
  
<span data-ttu-id="ef9dd-112">ユーザーが自分のメールボックスでメールの転送をセットアップできるように、セットアップ手順をユーザーに送信するには、[Microsoft 365 から別のメール アカウントにメールを転送する](https://support.office.com/article/Forward-email-from-Office-365-to-another-email-account-1ed4ee1e-74f8-4f53-a174-86b748ff6a0e)ように指示します。</span><span class="sxs-lookup"><span data-stu-id="ef9dd-112">To send instructions to your users so they can set up email forwarding on their own mailboxes, point them to [Forward email from Microsoft 365 to another email account](https://support.office.com/article/Forward-email-from-Office-365-to-another-email-account-1ed4ee1e-74f8-4f53-a174-86b748ff6a0e).</span></span> <span data-ttu-id="ef9dd-113">転送は、1 つのメール アドレスに対してのみ可能な点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="ef9dd-113">Please note that you can forward to only one email address.</span></span> <span data-ttu-id="ef9dd-114">ユーザーのグループへの転送をセットアップする必要がある場合は、配布リスト ([**グループ**] の下) を作成し、配布リストにユーザーを追加し、そのグループへの転送を構成します。</span><span class="sxs-lookup"><span data-stu-id="ef9dd-114">If you need to set up forwarding to a group of people, create a distribution list (under **Groups**), add your users to it, and then configure forwarding to that group.</span></span>
  
<span data-ttu-id="ef9dd-115">従業員が退職する場合</span><span class="sxs-lookup"><span data-stu-id="ef9dd-115">Do you have an employee leaving?</span></span> <span data-ttu-id="ef9dd-116">推奨される手順については、「[Microsoft 365 から元従業員を削除する](https://docs.microsoft.com/microsoft-365/admin/add-users/remove-former-employee)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ef9dd-116">See [Remove a former employee from Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/remove-former-employee) for the recommended steps.</span></span>