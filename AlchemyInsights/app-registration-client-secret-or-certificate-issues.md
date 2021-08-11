---
title: アプリ登録クライアントの秘密または証明書の問題
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
- "9004352"
- "9685"
ms.openlocfilehash: 588273f43f7c2d57b377b234885cf4283d466919b562536f78a64356422f9f9f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951498"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a>アプリ登録クライアントの秘密または証明書の問題

アプリケーション クライアント シークレットの有効期限が切れていますか?

登録されたアプリケーションがどのように作成されたかに関係なく、アプリ登録ポータルでの標準の登録プロセスを通じて、またはアプリケーションの同意を使用してサービス プリンシパルがテナントで作成されたかどうかに関係なく、新しいクライアント シークレットは、現在のクライアント シークレットの有効期限が切れる前に作成し、関連するアプリケーション コードで更新する必要があります。 最大有効期間は 2 年です。 ポータルのアプリ登録ページを離れると表示されなくなるため、シークレット値を記録する必要があります。 詳細については、「[クイックスタート: Microsoft ID プラットフォームへのアプリの登録](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app)」および「[Microsoft ID プラットフォームのベスト プラクティス](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)」を参照してください。

詳細については、「[ポータルでの Azure AD アプリとサービス プリンシパルの作成 - Microsoft ID プラットフォーム](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)」を参照してください。
