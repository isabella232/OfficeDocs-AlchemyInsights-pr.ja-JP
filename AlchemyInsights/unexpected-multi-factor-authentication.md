---
title: 予期しない多要素認証
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ''
ms.custom:
- "1300007"
- "4372"
ms.openlocfilehash: 8a912b32dee23e8c6eae0ad7bc72228d49ceeb92
ms.sourcegitcommit: 4f7ff981bbb3a98663cd164d0a10bb082cdf7ec9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948819"
---
# <a name="unexpected-multi-factor-authentication"></a><span data-ttu-id="ef28b-102">予期しない多要素認証</span><span class="sxs-lookup"><span data-stu-id="ef28b-102">Unexpected multi-factor authentication</span></span>

<span data-ttu-id="ef28b-103">2019 年 10 月 21 日以降にテナントが作成され、予期せず MFA の入力を求められた場合は、テナントで[セキュリティの既定](http://aka.ms/securitydefaults)が有効になっている可能性があります。</span><span class="sxs-lookup"><span data-stu-id="ef28b-103">If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](http://aka.ms/securitydefaults) enabled in your tenant.</span></span> 

<span data-ttu-id="ef28b-104">セキュリティの既定値を管理するには:</span><span class="sxs-lookup"><span data-stu-id="ef28b-104">To Manage security defaults:</span></span>

1. <span data-ttu-id="ef28b-105">グローバル管理者の資格情報を使用して、[管理センター](https://go.microsoft.com/fwlink/p/?linkid=834822)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="ef28b-105">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="ef28b-106">[Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties) にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="ef28b-106">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="ef28b-107">ページの下部で、[**セキュリティの既定値の管理**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="ef28b-107">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="ef28b-108">セキュリティの規定値を有効にするには [**はい**] をクリックし、セキュリティの規定値を無効にするには [**いいえ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="ef28b-108">Click **Yes** to enable security defaults and **No** to disable security defaults.</span></span>
