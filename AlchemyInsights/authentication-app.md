---
title: 認証アプリ
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405851"
---
# <a name="authentication-app"></a><span data-ttu-id="1dcc8-102">認証アプリ</span><span class="sxs-lookup"><span data-stu-id="1dcc8-102">Authentication app</span></span>

<span data-ttu-id="1dcc8-103">グローバル管理者の場合、[サインイン診断](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)を使用して、ユーザーのサインインに関連して何が起こったかをすばやく調べたり、問題を診断したりできます。</span><span class="sxs-lookup"><span data-stu-id="1dcc8-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="1dcc8-104">「[診断の起動](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)」ボタンをクリックして診断を開始します。</span><span class="sxs-lookup"><span data-stu-id="1dcc8-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="1dcc8-105">ユーザー、アプリケーション、サインイン時間、リクエスト ID、または相関 ID に関する詳細を入力して、分析するイベントを見つけます。</span><span class="sxs-lookup"><span data-stu-id="1dcc8-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="1dcc8-106">何が起こったかの詳細と、変更が必要な場合に変更を加えるために実行できるアクションを示す診断結果を確認します。</span><span class="sxs-lookup"><span data-stu-id="1dcc8-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="1dcc8-107">**該当するシナリオを確認してください。**</span><span class="sxs-lookup"><span data-stu-id="1dcc8-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="1dcc8-108">ユーザーが Microsoft Authenticator アプリでプッシュ通知を受け取らない場合は、「[ユーザーのブロックとブロック解除](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)」の説明に従って、MFA ブロックされたユーザーの下にプッシュ通知が表示されていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="1dcc8-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="1dcc8-109">ユーザーが MFA でブロックされていないが、プッシュ通知を受信しない場合、ユーザーは Microsoft Authenticator アプリを開くことができます。これにより、保留中の承認要求がプルされます。</span><span class="sxs-lookup"><span data-stu-id="1dcc8-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="1dcc8-110">別のサインイン方法として、ユーザーは別の方法で [サインイン] をクリックして、モバイル アプリから確認コードを使用することを選択することもできます。</span><span class="sxs-lookup"><span data-stu-id="1dcc8-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="1dcc8-111">Microsoft Authenticator アプリは、多くのユーザーが利用できる唯一の方法です。</span><span class="sxs-lookup"><span data-stu-id="1dcc8-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="1dcc8-112">[セキュリティのデフォルトの詳細](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)については、[Authenticator App のよくある質問](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq)と、それらを解決する方法を確認してください。</span><span class="sxs-lookup"><span data-stu-id="1dcc8-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="1dcc8-113">**推奨ビデオ**</span><span class="sxs-lookup"><span data-stu-id="1dcc8-113">**Recommended Videos**</span></span>

<span data-ttu-id="1dcc8-114">[新しい電話で認証システム アプリを設定する方法 (2 分)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)。</span><span class="sxs-lookup"><span data-stu-id="1dcc8-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
