---
title: API アクセス許可と同意
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
- "9004343"
- "7756"
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932102"
---
# <a name="api-permissions-and-consent"></a>API アクセス許可と同意

Microsoft ID プラットフォームと統合するアプリケーションは、ユーザーと管理者がデータへのアクセス方法を制御できる承認モデルに従います。 承認モデルの実装は、Microsoft ID プラットフォーム エンドポイントで更新されています。 これにより、アプリが Microsoft ID プラットフォームを操作する方法が変更されます。 「[Microsoft ID プラットフォーム エンドポイントのアクセス許可と同意](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)」は、スコープ、アクセス許可、同意など、この承認モデルの基本的な概念を網羅しています。

[Azure Active Directory (Azure AD) 同意フレームワーク](https://docs.microsoft.com/azure/active-directory/develop/consent-framework)を使用すると、マルチテナント Web およびネイティブ クライアント アプリケーションを簡単に開発できます。 これらのアプリケーションでは、アプリケーションが登録されているものとは異なる Azure AD テナントからのユーザー アカウントによるサインインが可能です。 また、独自の Web API に加えて、Microsoft Graph API (Azure AD、Intune、および Microsoft 365 のサービスにアクセスするため) やその他の Microsoft サービスの API などの Web API にアクセスする必要がある場合もあります。

