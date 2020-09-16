---
title: トラブルシューティングの問題 - ディレクトリにユーザーが見つかりません
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725412"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="8f2c7-102">トラブルシューティングの問題 - ディレクトリにユーザーが見つかりません</span><span class="sxs-lookup"><span data-stu-id="8f2c7-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="8f2c7-103">ディレクトリに "ユーザーが見つかりません" というエラーメッセージが表示されている場合は、問題の種類が、"ディレクトリ内にユーザーが見つかりません" のときにもう一度お試しください。</span><span class="sxs-lookup"><span data-stu-id="8f2c7-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="8f2c7-104">問題のトラブルシューティングを行うには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="8f2c7-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="8f2c7-105">メール招待状を受諾したアカウントが、後でサインインするために使用しているアカウントと同じであることを確認します。</span><span class="sxs-lookup"><span data-stu-id="8f2c7-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="8f2c7-106">ユーザーが招待を承諾してサイトにサインインするために同じアカウントを使用していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="8f2c7-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="8f2c7-107">詳細については、[「Microsoft 365 ログインを管理するために Microsoft アカウント</a>のエイリアスを管理する方法」](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8f2c7-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="8f2c7-108">ユーザーがエラーを受信している各サイトに移動します。</span><span class="sxs-lookup"><span data-stu-id="8f2c7-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="8f2c7-109">サイト URL の末尾に "/_layouts/15/people.aspx/membershipgroupid = 0" (二重引用符内) を追加します。</span><span class="sxs-lookup"><span data-stu-id="8f2c7-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="8f2c7-110">例: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0。</span><span class="sxs-lookup"><span data-stu-id="8f2c7-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="8f2c7-111">一覧からユーザーを選択します。</span><span class="sxs-lookup"><span data-stu-id="8f2c7-111">Select the user from the list.</span></span>

- <span data-ttu-id="8f2c7-112">[**ユーザー権限の削除**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="8f2c7-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="8f2c7-113">ユーザーを追加して、ユーザーに招待状を再送信します。</span><span class="sxs-lookup"><span data-stu-id="8f2c7-113">Add back the User and Resend the invite to the user.</span></span>

