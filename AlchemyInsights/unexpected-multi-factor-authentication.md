---
title: 予期しない多要素認証
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ''
ms.custom:
- "1300007"
- "4372"
ms.openlocfilehash: 48303d5b408cbdb243ec45dc4c80ac9a83f273a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689527"
---
# <a name="unexpected-multi-factor-authentication"></a><span data-ttu-id="e46b3-102">予期しない多要素認証</span><span class="sxs-lookup"><span data-stu-id="e46b3-102">Unexpected multi-factor authentication</span></span>

<span data-ttu-id="e46b3-103">2019 年 10 月 21 日以降にテナントが作成され、予期せず MFA の入力を求められた場合は、テナントで[セキュリティの既定](https://aka.ms/securitydefaults)が有効になっている可能性があります。</span><span class="sxs-lookup"><span data-stu-id="e46b3-103">If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span> 

<span data-ttu-id="e46b3-104">セキュリティの既定値を管理するには:</span><span class="sxs-lookup"><span data-stu-id="e46b3-104">To Manage security defaults:</span></span>

1. <span data-ttu-id="e46b3-105">グローバル管理者の資格情報を使用して、[管理センター](https://go.microsoft.com/fwlink/p/?linkid=834822)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="e46b3-105">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="e46b3-106">[Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties) にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="e46b3-106">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="e46b3-107">ページの下部で、[**セキュリティの既定値の管理**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="e46b3-107">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="e46b3-108">セキュリティの規定値を有効にするには [**はい**] をクリックし、セキュリティの規定値を無効にするには [**いいえ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="e46b3-108">Click **Yes** to enable security defaults and **No** to disable security defaults.</span></span>
