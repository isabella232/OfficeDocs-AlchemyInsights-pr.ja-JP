---
title: Mac 用の Teams アドイン
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670333"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="83557-102">Mac 用の Teams アドイン</span><span class="sxs-lookup"><span data-stu-id="83557-102">Teams add-in for Mac</span></span>

<span data-ttu-id="83557-103">Mac オペレーティング システム ユーザー用の Teams アドインが存在しない問題のトラブルシューティングを行うには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="83557-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="83557-104">**手順 1:** Hybrid Exchange オンプレミス（2016 CU3 以降に必要）を所有している場合は、 Test-HMA.ps1 ツールを使用してハイブリッド先進認証が正しく構成されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="83557-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="83557-105">詳細については、[「iOS および Android 用の Outlook でのハイブリッド先進認証の検証」](https://aka.ms/AA980zq) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="83557-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="83557-106">**注:** domain\username ではなく、UPN のアドレス形式（たとえば、[username@contoso.com](mailto:username@contoso.com)）を使用してください。</span><span class="sxs-lookup"><span data-stu-id="83557-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="83557-107">Exchange Online メールボックスを使用するユーザーの場合でも、この操作を行います。</span><span class="sxs-lookup"><span data-stu-id="83557-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="83557-108">**手順 2:** **ツール** > **アカウント**に移動します。Mac 用 Outlook で、アカウントを見つけて選択します。</span><span class="sxs-lookup"><span data-stu-id="83557-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="83557-109">表示されているユーザー名が[username@contoso.com](mailto:username@contoso.com) のような UPN 形式であることを確認します。</span><span class="sxs-lookup"><span data-stu-id="83557-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="83557-110">**手順 3:** ユーザーがライセンス認証を受けた Microsoft Teams ユーザーであることを確認します。</span><span class="sxs-lookup"><span data-stu-id="83557-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="83557-111">ユーザーは、Mac 用 Office 365 サブスクリプションの製品バージョン 16.24 以降を使用している必要があります。</span><span class="sxs-lookup"><span data-stu-id="83557-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>