---
title: Azure AD に参加しているデバイスのシングル サインオンのトラブルシューティング
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
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2021
ms.locfileid: "51038283"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Azure AD に参加しているデバイスのシングル サインオンのトラブルシューティング

オンプレミスの Active Directory (AD) 環境があり、AD ドメイン参加済みのコンピューターを Azure AD に参加させたい場合、「 ハイブリッド Azure AD 参加」を行うことで実現できます。 [方法: ハイブリッド Azure Active Directory 参加の実装計画](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan)では、環境にハイブリッド Azure AD 参加を実装するための関連する手順を提供します。

詳細については、「[Windows Hello for Business を使用して Azure AD に参加しているデバイスをオンプレミスのシングル サインオン用に構成する](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)」を参照してください。

**プライマリ 更新トークン (PRT) 問題**

プライマリ 更新トークン (PRT) は、Windows 10、Windows Server 2016 以降のバージョン、iOS、Android デバイス上の Azure AD 認証の主要な成果物です。 これは、Microsoft のファースト パーティ トークン ブローカーに特別に発行される JSON Web トークン (SSO) であり、これらのデバイスで使用されるアプリケーション全体でシングル サインオン (SSO) が有効になります。 Windows 10 デバイスで PRT が発行、使用、保護される方法の詳細については、「[プライマリ リフレッシュ トークンとは](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)」を参照してください。 

**WamDefaultSet: YES および AzureADSet: YES**

これらのフィールドは、デバイスにサインインするときに、ユーザーが Azure AD に対して正常に認証されたかどうかを示します。 値が [**いいえ**] の場合、次の原因が考えられます。

- 登録時にデバイスに関連付けられている TPM のストレージ キーが正しくありません (管理者特権の実行中に、KeySignTest を確認してください)
- 代替ログイン ID
- HTTP プロキシが見つかりません

dsregcmd コマンドを使用してデバイスのトラブルシューティングを行うには、「[SSOの状態](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)」を参照してください。
