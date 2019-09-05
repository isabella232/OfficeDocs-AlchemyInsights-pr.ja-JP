---
title: 問題のトラブルシューティング-ディレクトリにユーザーがありません
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754197"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="b9faf-102">問題のトラブルシューティング-ディレクトリにユーザーがありません</span><span class="sxs-lookup"><span data-stu-id="b9faf-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="b9faf-103">ユーザーがディレクトリに "ユーザーが見つかりません" というエラーメッセージが表示される場合。</span><span class="sxs-lookup"><span data-stu-id="b9faf-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="b9faf-104">問題の種類がディレクトリ内にない場合は、もう一度やり直してください。</span><span class="sxs-lookup"><span data-stu-id="b9faf-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="b9faf-105">問題のトラブルシューティングを行うには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="b9faf-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="b9faf-106">電子メール招待状を受諾したアカウントが、後でサインインするために使用されているのと同じアカウントであることを確認します。</span><span class="sxs-lookup"><span data-stu-id="b9faf-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="b9faf-107">ユーザーが同じアカウントを使用して、招待状を承諾してサイトにサインインしていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="b9faf-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="b9faf-108">詳細については、「 [office 365 ログインを管理する</a>ために Microsoft アカウントのエイリアスを管理する方法](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b9faf-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="b9faf-109">ユーザーがエラーを受信している各サイトを参照します。</span><span class="sxs-lookup"><span data-stu-id="b9faf-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="b9faf-110">サイト URL の末尾に "/_layouts/15/people.aspx/membershipgroupid = 0" (二重引用符内) を追加します。</span><span class="sxs-lookup"><span data-stu-id="b9faf-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="b9faf-111">例: https://< "contoso" ></span><span class="sxs-lookup"><span data-stu-id="b9faf-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="b9faf-112">リストからユーザーを選択します。</span><span class="sxs-lookup"><span data-stu-id="b9faf-112">Select the user from the list.</span></span>

- <span data-ttu-id="b9faf-113">リボンから [**ユーザー権限の削除**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="b9faf-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="b9faf-114">ユーザーを再度追加して、招待状を再送信します。</span><span class="sxs-lookup"><span data-stu-id="b9faf-114">Add back the User and Resend the invite to the user.</span></span>

