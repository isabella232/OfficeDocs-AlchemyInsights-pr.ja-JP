---
title: トークンの有効期限の構成と延長
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: ce100fcc2c62d62477f78e10b3cc9233fc2f5c5b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329091"
---
# <a name="configure-and-extend-token-lifetimes"></a>トークンの有効期限の構成と延長

Microsoft ID プラットフォームによって発行されるアクセス、SAML、または ID トークンの有効期限を指定できます。 組織のすべてのアプリ、マルチテナント (多組織) アプリケーション、組織の特定のサービス プリンシパルにトークンの有効期間を設定できます。 詳細については、「[構成可能なトークンの有効期限](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)」を参照してください。

たとえば、「[トークンの有効期限の構成例](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes)」を参照してください。

Azure Active Directory B2C (Azure AD B2C) のトークンの有効期限と互換性を構成する方法については、「[Azure Active Directory B2C でトークンを構成する](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow)」を参照してください。

記事「[Azure Active Directory B2C でのセッション動作を構成する](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow)」では、Azure AD B2C で使用されるシングル サインオン (SSO) 方式について説明し、ポリシーを構成するときに最適な SSO 方式を選択するのに役立ちます。

**トークンの有効期間はどのぐらいですか?いつまで有効ですか?**

トークンの有効期限は 1 時間、セッションの有効期限は 24 時間です。 つまり、24 時間以内に要求が行われなかった場合は、新しいトークンを要求する前に再度ログインする必要があります。

**注**: 2020 年 5 月 30 日を過ぎると、新しいテナントは構成可能なトークンの有効期間ポリシーを使用してセッションおよびトークンの更新を構成できなくなります。 その後数ヶ月以内に廃止されるため、既存のセッションの承認を停止し、トークン ポリシーを更新します。 廃止された後も、アクセス トークンの有効期限を構成できます。






