---
title: 条件付きアクセス ポリシー
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: af95627d07d41add54f03c9254562b9be4e05d9b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817285"
---
# <a name="conditional-access-policies"></a><span data-ttu-id="441cf-102">条件付きアクセス ポリシー</span><span class="sxs-lookup"><span data-stu-id="441cf-102">Conditional Access policies</span></span>

<span data-ttu-id="441cf-103">条件付きアクセスとは、環境内のアプリへのアクセスを特定の条件に基づいて制御する、中央の場所から管理される Azure AD の機能のことです。</span><span class="sxs-lookup"><span data-stu-id="441cf-103">Conditional Access is a capability of Azure AD that enables you to enforce controls on the access to apps in your environment, all based on specific conditions and managed from a central location.</span></span>

<span data-ttu-id="441cf-104">詳細については「[Azure AD 条件付きアクセス](https://docs.microsoft.com/azure/active-directory/conditional-access/)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="441cf-104">Learn more about [Azure AD Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>  

<span data-ttu-id="441cf-105">**注**: 2019 年 10 月 21 日以降にテナントが作成され、予期せず MFA の入力を求められた場合は、テナントで [セキュリティの既定](https://aka.ms/securitydefaults)が有効になっている可能性があります。</span><span class="sxs-lookup"><span data-stu-id="441cf-105">**Note**: If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span>

<span data-ttu-id="441cf-106">**セキュリティの既定値を管理するには**</span><span class="sxs-lookup"><span data-stu-id="441cf-106">**To Manage security defaults**</span></span>

1. <span data-ttu-id="441cf-107">グローバル管理者の資格情報を使用して、[管理センター](https://go.microsoft.com/fwlink/p/?linkid=834822)にサインインします。</span><span class="sxs-lookup"><span data-stu-id="441cf-107">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="441cf-108">[Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties) にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="441cf-108">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="441cf-109">ページの下部で、[**セキュリティの既定値の管理**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="441cf-109">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="441cf-110">セキュリティの既定値を有効にするには **[はい]** をクリックし、セキュリティの既定値を無効にするには **[いいえ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="441cf-110">Click **Yes** to enable security defaults or **No** to disable security defaults.</span></span>
