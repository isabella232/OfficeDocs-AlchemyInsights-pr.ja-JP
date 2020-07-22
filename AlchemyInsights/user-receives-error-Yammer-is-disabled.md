---
title: ユーザーが受け取ったエラー AADSTS7000112 Yammer が無効になっています
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198654"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="23beb-102">ユーザーが受け取ったエラー AADSTS7000112 Yammer が無効になっています</span><span class="sxs-lookup"><span data-stu-id="23beb-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="23beb-103">エラー「AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled」を受け取った場合は、Azure AD 内のサービスプリンシパルに問題があります。</span><span class="sxs-lookup"><span data-stu-id="23beb-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="23beb-104">管理者がサービスプリンシパルを無効にして、Yammer へのアクセスをブロックしている可能性があります。</span><span class="sxs-lookup"><span data-stu-id="23beb-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="23beb-105">サービスプリンシパルを無効にすることはお勧めできません。別の問題が発生する恐れがあります。</span><span class="sxs-lookup"><span data-stu-id="23beb-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="23beb-106">Yammer へのユーザーアクセスをブロックするためにサポートされているアプローチの詳細については、「[Microsoft 365ユーザーのYammer アクセスを無効にする](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="23beb-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="23beb-107">Azure Portal でこの問題を修正し、Yammer へのユーザーアクセスを復元するには：</span><span class="sxs-lookup"><span data-stu-id="23beb-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="23beb-108">Azure Active Directory ページを開き、左側のナビゲーションウィンドウの[**管理**]で[**エンタープライズアプリケーション**]を選択します。</span><span class="sxs-lookup"><span data-stu-id="23beb-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="23beb-109">検索ボックスに「\*\* Office 365 Yammer \*\*」と入力し、アプリケーション名を選択して設定を開きます。</span><span class="sxs-lookup"><span data-stu-id="23beb-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="23beb-110">左側のナビゲーションウィンドウの[**管理**]で[**プロパティ**]を選択します。</span><span class="sxs-lookup"><span data-stu-id="23beb-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="23beb-111">[**ユーザーがログインできるようにしますか?**]の値を[**はい**]に設定して、[**保存**]を選択します。</span><span class="sxs-lookup"><span data-stu-id="23beb-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="23beb-112">Yammer に再度サインインします。</span><span class="sxs-lookup"><span data-stu-id="23beb-112">Sign in to Yammer again.</span></span> <span data-ttu-id="23beb-113">クッキーを消去する必要があるかもしれません。</span><span class="sxs-lookup"><span data-stu-id="23beb-113">You might need to clear cookies.</span></span>

<span data-ttu-id="23beb-114">または、PowerShell コマンドを実行して値を設定します。</span><span class="sxs-lookup"><span data-stu-id="23beb-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="23beb-115">詳細については、Office 365 で Yammer タイルをクリックする際に発生するエラー[「Sorry, but we're having trouble signing you in」](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="23beb-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 