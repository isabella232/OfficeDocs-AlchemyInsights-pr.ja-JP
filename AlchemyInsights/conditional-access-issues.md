---
title: 条件付きアクセスの問題
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015070"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="83361-102">条件付きアクセスの問題</span><span class="sxs-lookup"><span data-stu-id="83361-102">Conditional access issues</span></span>

<span data-ttu-id="83361-103">**サインイン診断で問題を解決する**</span><span class="sxs-lookup"><span data-stu-id="83361-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="83361-104">[サインイン診断](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)を使用すると、ユーザーのサインインに関連して何が起こったかをすばやく調べたり、問題を診断したりできます。</span><span class="sxs-lookup"><span data-stu-id="83361-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="83361-105">[サインイン診断] を起動します。</span><span class="sxs-lookup"><span data-stu-id="83361-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="83361-106">ユーザー、アプリケーション、サインイン時間、リクエスト ID、または相関 ID に関する詳細を入力して、分析するイベントを見つけます。</span><span class="sxs-lookup"><span data-stu-id="83361-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="83361-107">何が起こったかの詳細と、(変更が必要な場合に) 変更を加えるために実行できるアクションを示す診断結果を確認します。</span><span class="sxs-lookup"><span data-stu-id="83361-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="83361-108">**サインインのトラブルシューティング手順**</span><span class="sxs-lookup"><span data-stu-id="83361-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="83361-109">Azure AD サインイン ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="83361-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="83361-110">サインインをユーザー、時間範囲、アプリケーション、ステータス、クライアント アプリなどでフィルタリングします。</span><span class="sxs-lookup"><span data-stu-id="83361-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="83361-111">サインイン イベントを選択し、[条件付きアクセス] タブを表示して、評価されたポリシーを確認します。</span><span class="sxs-lookup"><span data-stu-id="83361-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="83361-112">ポリシーの行をクリックして、ポリシーの詳細を表示し、ポリシーが適用された理由を理解します。</span><span class="sxs-lookup"><span data-stu-id="83361-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="83361-113">**条件付きアクセス ポリシーのトラブルシューティングを行うためのツール**</span><span class="sxs-lookup"><span data-stu-id="83361-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="83361-114">[レポートのみ] モードでは、ユーザーに影響を与えることなくポリシーを評価できます。</span><span class="sxs-lookup"><span data-stu-id="83361-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="83361-115">What-if ツールを使用すると、サインイン イベントをシミュレートし、適用されるポリシーを確認できます。</span><span class="sxs-lookup"><span data-stu-id="83361-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="83361-116">インサイトとレポート ワークブックには、各ポリシーのリアルタイムの影響が表示されます。</span><span class="sxs-lookup"><span data-stu-id="83361-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="83361-117">**ベースライン保護ポリシー**</span><span class="sxs-lookup"><span data-stu-id="83361-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="83361-118">ベースライン保護ポリシーは非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="83361-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="83361-119">これらは強制でなくなり、間もなく Azure ポータルから削除されます。</span><span class="sxs-lookup"><span data-stu-id="83361-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="83361-120">[セキュリティの既定値](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)を有効にすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="83361-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="83361-121">条件付きアクセスの詳細については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="83361-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="83361-122">[Azure Active Directory での条件付きアクセスのベストプ ラクティス](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[条件付きアクセスの条件](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[条件付きアクセスの制御](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[条件付きアクセスの場所](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="83361-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
