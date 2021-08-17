---
title: SSPR のトラブルシューティング
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 9d8184efdc60befd359059c62ea3eb1a14ad7d2a20dade921d4a71e424f52033
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038963"
---
# <a name="troubleshoot-sspr"></a>SSPR のトラブルシューティング

**パスワードのリセットの構成に問題がある**

- お客様が管理者であり、セルフサービスによるパスワードのリセットを有効にする方法を探している場合は、「[SSPR を有効にするためのチュートリアル](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)」を参照して、組織のパスワードのリセットを構成してください。 「[ライセンス要件](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)」もご確認ください。 組織内で少なくとも 1 つのライセンスが割り当てられている必要があります。
    - **クラウド専用ユーザー** - 任意の Office 365 (O365) 有料 SKU または Azure AD Basic
    - **クラウドとオンプレミス ユーザー** - Azure AD Premium P1 または P2、Enterprise Mobility + Security (EMS)、または Secure Productive Enterprise (SPE)
- セルフサービスによるパスワードのリセットに関するその他の質問については、「[FAQ](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)」を参照してください。

**次のエラー メッセージが表示されます**

一般的なエラーとその解決策を見つけるには、以下の記事を参照してください。「[セルフサービスによるパスワードのリセットのトラブルシューティングを行う](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)」

**パスワードのリセット ポリシーに問題がある**

- パスワード のリセット ポリシーが期待どおりに動作しない場合、またはパスワードのリセット ポリシーについて質問がある場合は、「[Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)のパスワード ポリシーと制限」を参照してください。
- パスワード リセット ポリシーは、管理者には適用されません。 Microsoft は Azure 管理者の役割に、強力な既定の 2 ゲート パスワード リセット ポリシーを適用しています。 管理者ではないユーザーでテストを行うようにしてください。 管理者のリセット ポリシーの詳細については、「[管理者のリセット ポリシーの違い](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)」を参照してください。

**ユーザーにパスワードのリセットに関する追加のセキュリティ情報を登録させない**

API、PowerShell、または Azure AD Connect を使用して、ユーザーのデータ (メールと電話の属性) を事前に設定することができます。 具体的な方法については、以下を参照してください。

- [ユーザーに登録を求めることなくパスワードのリセットを展開する](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [パスワードのリセットで使用されるデータ](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**ユーザーにパスワードの再設定のために追加のセキュリティ情報を登録してもらいたい**

1. ユーザーを [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info) に誘導して、セルフサービスによるパスワードのリセットのためのセキュリティ情報を登録してもらいます。
1. (ユーザーまたは管理者によって) ユーザーのデータが入力されたら、ユーザーに [aka.ms/sspr](https://passwordreset.microsoftonline.com/) に誘導し、ユーザーが自分でパスワードをリセットできるようにします。
1. ユーザーに引き続き問題が発生する場合は、**フェデレーション** ユーザーまたは **パスワード ハッシュが同期された** ユーザーである可能性があります。 つまり、パスワード Writeback サービスに問題がある可能性があります。