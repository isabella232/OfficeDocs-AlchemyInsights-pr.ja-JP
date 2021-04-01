---
title: Azure Active Directory に参加しているデバイスのシングル サインオン
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
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405849"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Azure Active Directory に参加しているデバイスのシングル サインオン

オンプレミスの Active Directory (AD) 環境があり、AD ドメイン参加済みのコンピューターを Azure AD に参加させたい場合、「 ハイブリッド Azure AD 参加」を行うことで実現できます。 [方法: ハイブリッド Azure Active Directory 参加の実装計画](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan)では、環境にハイブリッド Azure AD 参加を実装するための関連する手順を提供します。

[Windows Hello for Business を使用して Azure AD に参加しているデバイスをオンプレミスのシングル サインオン用に構成する](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**プライマリ 更新トークン (PRT) が発行** プライマリ 更新トークン (PRT) は、Windows 10、Windows Server 2016 以降のバージョン、iOS、Android デバイス上の Azure AD 認証の主要な成果物です。 これは、Microsoft のファースト パーティ トークン ブローカーに特別に発行される JSON Web トークン (SSO) であり、これらのデバイスで使用されるアプリケーション全体でシングル サインオン (SSO) が有効になります。 「[プライマリ リフレッシュ トークンとは?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)」では、Windows 10 デバイスで PRT が発行、使用、保護される方法の詳細を説明しています。

**WamDefaultSet: YES および AzureADPrt: YES** これらのフィールドは、デバイスにサインインするときに、ユーザーが Azure AD に対して正常に認証されたかどうかを示します。 値が [**いいえ**] の場合、次の原因が考えられます。

- 登録時にデバイスに関連付けられている TPM のストレージ キーが正しくありません (管理者特権の実行中に、KeySignTest を確認してください)。
- 代替ログイン ID
- HTTP プロキシが見つかりません

dsregcmd コマンドを使用してデバイスのトラブルシューティングを行う -[SSOの状態](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
