---
title: 管理者の同意の問題
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 08d3bfa84fd5ab31d7165090c392866d863898545ade7631e820a100eef89dea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952578"
---
# <a name="admin-consent-issues"></a>管理者の同意の問題

1. [管理者同意ワークフロー](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow)を有効にして、ユーザーが同意画面から直接管理者の承認を要求できるようにします。

1. 同意プロセス中にあなたまたはアプリケーションのユーザーに予期しないエラーが表示される場合は、トラブルシューティング手順について次の記事を参照してください：[「アプリケーションに同意すると、予期しないエラーが発生する」](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)。

1. [Microsoft ID プラットフォームでの管理者の同意](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)、[同意プロンプト](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)の仕組み、および[テナント全体の管理者の同意の要求を評価する](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)方法の詳細をご覧ください。

1. Microsoft ID プラットフォームと統合するアプリケーションは、ユーザーと管理者がデータへのアクセス方法を制御できる承認モデルに従います。 承認モデルの実装は、Microsoft ID プラットフォームエンドポイントで更新され、それにより、アプリが Microsoft ID プラットフォームと対話する方法が変更されました。 スコープ、アクセス許可、同意など、この承認モデルの概要については、「[Microsoft ID プラットフォーム エンドポイントのアクセス許可と同意](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)」を参照してください。