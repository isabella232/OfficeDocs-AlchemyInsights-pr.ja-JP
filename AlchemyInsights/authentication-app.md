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
ms.openlocfilehash: 1ac3158914455502d2de493dd1320034b1d09573ebb3ffef24c23eb1e816cad0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082947"
---
# <a name="authentication-app"></a>認証アプリ

グローバル管理者の場合、[サインイン診断](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)を使用して、ユーザーのサインインに関連して何が起こったかをすばやく調べたり、問題を診断したりできます。

1. 「[診断の起動](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)」ボタンをクリックして診断を開始します。 
1. ユーザー、アプリケーション、サインイン時間、リクエスト ID、または相関 ID に関する詳細を入力して、分析するイベントを見つけます。
1. 何が起こったかの詳細と、変更が必要な場合に変更を加えるために実行できるアクションを示す診断結果を確認します。

**該当するシナリオを確認してください。**

1. ユーザーが Microsoft Authenticator アプリでプッシュ通知を受け取らない場合は、「[ユーザーのブロックとブロック解除](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)」の説明に従って、MFA ブロックされたユーザーの下にプッシュ通知が表示されていないことを確認します。
1. ユーザーが MFA でブロックされていないが、プッシュ通知を受信しない場合、ユーザーは Microsoft Authenticator アプリを開くことができます。これにより、保留中の承認要求がプルされます。
1. 別のサインイン方法として、ユーザーは別の方法で [サインイン] をクリックして、モバイル アプリから確認コードを使用することを選択することもできます。
1. Microsoft Authenticator アプリは、多くのユーザーが利用できる唯一の方法です。 [セキュリティのデフォルトの詳細](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)については、[Authenticator App のよくある質問](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq)と、それらを解決する方法を確認してください。
 
**推奨ビデオ**

[新しい電話で認証システム アプリを設定する方法 (2 分)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)。
