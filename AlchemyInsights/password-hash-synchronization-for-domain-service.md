---
title: ドメイン サービスのパスワード ハッシュ同期
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 3c00105a67f70ae9ce11cd8bb922c4d84a320010d021414b9159948f7dc87dbc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040871"
---
# <a name="password-hash-synchronization-for-domain-service"></a>ドメイン サービスのパスワード ハッシュ同期

**Azure AD DS インスタンスがパスワード ハッシュ同期を有効にするように要求している場合**

オンプレミスの Azure Active Directory Domain Services (AD DS) 環境からユーザーが同期するハイブリッド環境を実行しているシナリオが発生します。 このシナリオは、オンプレミス AD DS から Azure AD テナントへのパスワード ハッシュ同期があるにもかかわらず発生します。

**原因**

これは、Azure AD Connect が既定で、Azure AD DS に必要な従来の New Technology LAN Manager (NTLM) と Kerberos パスワード ハッシュを同期しないために発生します。

**回避策** 

NTLM および Kerberos 認証に必要なパスワード ハッシュを同期するように Azure AD Connect を構成する必要があります。

Azure AD Connect が構成された後、オンプレミスのアカウント作成またはパスワード変更イベントも、従来のパスワード ハッシュを Azure AD に同期します。 これに関する詳細情報と、Azure AD DS ハイブリッド環境でパスワード同期を有効にする方法のガイダンスについては、[こちら](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync)を参照してください。