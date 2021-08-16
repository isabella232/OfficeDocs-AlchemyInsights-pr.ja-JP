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
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069969"
---
# <a name="conditional-access-issues"></a>条件付きアクセスの問題

**サインイン診断で問題を解決する**

[サインイン診断](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)を使用すると、ユーザーのサインインに関連して何が起こったかをすばやく調べたり、問題を診断したりできます。

1. [サインイン診断] を起動します。
1. ユーザー、アプリケーション、サインイン時間、リクエスト ID、または相関 ID に関する詳細を入力して、分析するイベントを見つけます。
1. 何が起こったかの詳細と、(変更が必要な場合に) 変更を加えるために実行できるアクションを示す診断結果を確認します。

**サインインのトラブルシューティング手順** 

1. Azure AD サインイン ページに移動します。
1. サインインをユーザー、時間範囲、アプリケーション、ステータス、クライアント アプリなどでフィルタリングします。
1. サインイン イベントを選択し、[条件付きアクセス] タブを表示して、評価されたポリシーを確認します。
1. ポリシーの行をクリックして、ポリシーの詳細を表示し、ポリシーが適用された理由を理解します。

**条件付きアクセス ポリシーのトラブルシューティングを行うためのツール**

- [レポートのみ] モードでは、ユーザーに影響を与えることなくポリシーを評価できます。
- What-if ツールを使用すると、サインイン イベントをシミュレートし、適用されるポリシーを確認できます。
- インサイトとレポート ワークブックには、各ポリシーのリアルタイムの影響が表示されます。

**ベースライン保護ポリシー**

ベースライン保護ポリシーは非推奨になりました。 これらは強制でなくなり、間もなく Azure ポータルから削除されます。 [セキュリティの既定値](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)を有効にすることをお勧めします。

条件付きアクセスの詳細については、以下を参照してください。

[Azure Active Directory での条件付きアクセスのベストプ ラクティス](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[条件付きアクセスの条件](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[条件付きアクセスの制御](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[条件付きアクセスの場所](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
