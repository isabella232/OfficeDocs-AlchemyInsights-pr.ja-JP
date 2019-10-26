---
title: 削除されたフォームを復元する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2547"
- "9000672"
ms.openlocfilehash: 185e8787454efc38f378cce6fd7bea06d453bc92
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/24/2019
ms.locfileid: "37681692"
---
# <a name="restore-a-deleted-form"></a><span data-ttu-id="788bb-102">削除されたフォームを復元する</span><span class="sxs-lookup"><span data-stu-id="788bb-102">Restore a deleted form</span></span>

<span data-ttu-id="788bb-103">Microsoft Forms のフォームを誤って削除してしまった場合は、フォームを復元することができます。</span><span class="sxs-lookup"><span data-stu-id="788bb-103">If you deleted a form in Microsoft Forms by accident, you can recover it.</span></span> <span data-ttu-id="788bb-104">削除されたフォームの所有者として Microsoft Forms にサインインします。</span><span class="sxs-lookup"><span data-stu-id="788bb-104">Sign in to Microsoft Forms as the owner of the deleted form.</span></span> <span data-ttu-id="788bb-105">[**ごみ箱**] を選択してから、回復するフォームを選択し、[**復元**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="788bb-105">Select the **Recycle Bin**, then select the form you want to recover and select **Restore**.</span></span> <span data-ttu-id="788bb-106">復元が完了したら、[**フォームに戻る**] ページの矢印を選択します。</span><span class="sxs-lookup"><span data-stu-id="788bb-106">Once restored, select the **Back to my Forms page** arrow.</span></span>

<span data-ttu-id="788bb-107">フォームの所有者のみが復元できます。</span><span class="sxs-lookup"><span data-stu-id="788bb-107">Only the owner of the form can recover it.</span></span> <span data-ttu-id="788bb-108">フォーム所有者のアカウントが無効になっているか、テナントから削除されている場合、グローバル管理者のみがフォームを回復できます。</span><span class="sxs-lookup"><span data-stu-id="788bb-108">If form owner's account was disabled or removed from the tenant, only the Global Administrator can recover the form.</span></span> <span data-ttu-id="788bb-109">グローバル管理者が復元を実行するには、Forms ライセンスが必要です。</span><span class="sxs-lookup"><span data-stu-id="788bb-109">The Global Administrator must have a Forms license to perform a restore.</span></span> <span data-ttu-id="788bb-110">ユーザー アカウントが無効になっているか、テナントから削除されてから 30 日以内に作成されたフォームのみを復元できます。</span><span class="sxs-lookup"><span data-stu-id="788bb-110">Only forms created within 30 days of the user account being disabled or removed from the tenant can be restored.</span></span>

<span data-ttu-id="788bb-111">テナントのグローバル管理者であり、削除または無効化されたアカウントでフォームを復元する場合は、次の URL **https://forms.office.com/Pages/delegatepage.aspx?originalowner=[メール アドレス]** で [メール アドレス] を削除または無効化されたユーザーのメール アドレスに置き換えます。たとえば、メール アドレスが johndoe@contoso.com の場合、URL は **https://forms.office.com/Pages/delegatepage.aspx?originalowner=johndoe@contoso.com** のようになります。</span><span class="sxs-lookup"><span data-stu-id="788bb-111">If you are the Global Administrator of the tenant, and you want to recover a form from an account that was deleted or disabled, replace [email address] with the email address of the deleted or disabled user in the following URL: **https://forms.office.com/Pages/delegatepage.aspx?originalowner=[email address]** For example, if your email address is johndoe@contoso.com, the URL would be: **https://forms.office.com/Pages/delegatepage.aspx?originalowner=johndoe@contoso.com**.</span></span> 

<span data-ttu-id="788bb-112">ユーザーの削除したフォームにアクセスしたら、移動するフォームを選択し、[**その他のフォームのアクション**] > [**移動**] の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="788bb-112">Once you have access to the user's deleted forms, select the form you want to move, and then select **More Form Actions** > **Move**.</span></span>

<span data-ttu-id="788bb-113">削除され、ユーザが組織から削除されたフォームを復元したい場合、グローバル管理者は Office 365 でユーザを復元し、そのユーザのパスワードをリセットしてからそのユーザーとしてログインしている間、別のアクティブなユーザーにフォームを移動することができます。</span><span class="sxs-lookup"><span data-stu-id="788bb-113">If you want to recover a form where it was deleted and the user was removed from the organization, a Global Administrator can choose to recover the user in Office 365, reset the password for that user, and then while logged in as that user, access the form to move it to another active user.</span></span> 