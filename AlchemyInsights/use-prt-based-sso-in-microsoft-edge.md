---
title: PRT を使用した Microsoft Edge でのシングル サインオン
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005624"
- "9657"
ms.openlocfilehash: f74c80947f885214b8af48561b278c445069cdd0
ms.sourcegitcommit: 9540ba561c98b511483d6f3264c43bbecbf9f4d5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2021
ms.locfileid: "51421246"
---
# <a name="use-prt-based-sso-in-microsoft-edge"></a><span data-ttu-id="348cc-102">PRT を使用した Microsoft Edge でのシングル サインオン</span><span class="sxs-lookup"><span data-stu-id="348cc-102">Use PRT-based SSO in Microsoft Edge</span></span>

<span data-ttu-id="348cc-103">[プライマリ更新トークン (PRT)](https://go.microsoft.com/fwlink/?linkid=2133632) とは、Windows 10、iOS、Android デバイスでの認証に使用される Azure Active Directory キーのことです。</span><span class="sxs-lookup"><span data-stu-id="348cc-103">A [Primary Refresh Token (PRT)](https://go.microsoft.com/fwlink/?linkid=2133632) is an Azure Active Directory key used for authentication on Windows 10, iOS, and Android devices.</span></span> <span data-ttu-id="348cc-104">PRT を使用すると、これらのデバイスで使用されるすべてのアプリケーションへのシングル サインオンを実現できます。</span><span class="sxs-lookup"><span data-stu-id="348cc-104">PRT enables SSO for all applications used on those devices.</span></span>

<span data-ttu-id="348cc-105">Microsoft Edge では、PRT を使用したシングル サインオンへのサポートが元からあり、追加の拡張子は必要はありません。</span><span class="sxs-lookup"><span data-stu-id="348cc-105">In Microsoft Edge, support for PRT-based SSO is native and requires no additional extensions.</span></span> <span data-ttu-id="348cc-106">Windows 10 RS3 以上では、サインインしているユーザーは PRT ベースのシングル サインオンをサポートする Web サイトに、この PRT を使用してシングル サインオンを取得します。</span><span class="sxs-lookup"><span data-stu-id="348cc-106">On Windows 10 RS3 and above, signed-in users will get SSO with the PRT to websites that support PRT-based SSO.</span></span>
