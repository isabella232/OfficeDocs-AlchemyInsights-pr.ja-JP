---
title: Oアプリケーションへのサインインに関する問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901721"
---
# <a name="issues-signing-in-to-applications"></a>Oアプリケーションへのサインインに関する問題

ユーザーのサインインに関連する原因を検出する、または問題を診断するには、次の手順を実行します。

1. [[サインイン診断]](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom) を起動します。
2. ユーザー、アプリケーション、サインイン時間、リクエスト ID、または相関 ID に関する詳細を入力して、分析するイベントを見つけます。
3. 何が起こったかの詳細と、変更が必要な場合に変更を加えるために実行できるアクションを示す診断結果を確認します。

以下は、アプリケーションにサインインするときに発生する可能性のある一般的な問題です。

1. 自分またはユーザーが **Azure AD のサインインを完了したが、予期しないプロンプトが表示される** - 記事「[アプリケーションにサインインするときに、予期しない同意プロンプトが表示される](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)」と、「[アプリケーションに同意すると、予期しないエラーが発生する](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)」を参照してください。
2. 自分またはユーザーが、**アプリケーションに直接サインインしたが、カスタム ポータルまたはアクセス パネルのディープ リンクからアプリケーションにサインインできない**: 「[Azure AD マイ アプリからのアプリケーションへのサインインに関する問題のトラブルシューティング](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)」を参照してください。
3. 自分またはユーザーが **Azure AD のサインインを完了したが、アプリケーションにエラーメッセージが表示され、ユーザーはサインイン フローを完了できない**: アプリが Azure AD が発行した応答を受け入れなかったことが原因です。 [以下の手順](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error)に従ってトラブルシューティングします。
4. 自分またはユーザーが、**パスワード シングル サインオン用に構成されたギャラリー以外のアプリケーションにサインインできない**: トラブルシューティングを行うには、[次の手順](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)のガイダンスに従ってください。
5. 自分またはユーザーが、**パスワード シングル サインオン用に構成された Azure AD ギャラリー アプリケーションにサインインできない**: トラブルシューティングを行うには、[次の手順](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)のガイダンスに従ってください。
6. 自分またはユーザーが **Microsoft アプリケーションにサインインできない**: トラブルシューティングを行うには、[次の手順](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)に従ってください。
7. 自分またはユーザーが、**フェデレーション シングル サインオン用に構成されたギャラリー以外のアプリケーションにサインインできない**: トラブルシューティングを行うには、[次の手順](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery)のガイダンスに従ってください。
8. 自分またはユーザーが、**フェデレーション シングル サインオン用に構成された Azure AD ギャラリー アプリケーションにサインインできない**: トラブルシューティングを行うには、[次の手順](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)のガイダンスに従ってください。
9. 自分またはユーザーが **カスタム開発されたアプリケーションにサインインできない**: トラブルシューティングを行うには、[次の手順](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)に従ってください。
10. 自分またはユーザーが **Azure AD アプリケーション プロキシを使用してオンプレミス アプリケーションにサインインできない**: トラブルシューティングを行うには、[次の手順](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy)に従ってください。

