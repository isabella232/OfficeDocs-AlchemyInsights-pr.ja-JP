---
title: 外部設定の管理
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: a988d792c51a81eac9aad3e8b2cd20fec9b2df51766f8919312e933a806e47ef
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114717"
---
# <a name="managing-external-settings"></a>外部設定の管理

**アナウンス**

- [2021 年 1 月 4 日以降、Google からの Web View サインイン サポートの廃止](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support)。 互換性のテストに関する Google のガイダンスに従って、アプリが影響を受けるかどうかをテストします
- コンシューマー Google アカウントでユーザーにサインインするときは、システム Web ビューまたはシステム ブラウザーを使用していることを確認してください。

**招待設定の管理**

適切な人が招待状を送信できるように[外部コラボレーション設定を構成したことを確認します](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)。

**ゲスト ユーザーのアクセス許可を管理する**

1. グローバル管理者は、[外部コラボレーション設定] ページでゲスト アクセス許可を構成することにより、Azure portal を介してディレクトリ内のゲスト アクセス許可を管理できます。[この設定の詳細をご覧ください](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support)。
2. ゲストが Teams や SharePoint などのアプリにアクセスできるようにする場合は、ゲスト アクセスを許可するようにそれらのアプリが構成されていることを確認してください。[Teams の設定](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support)と [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support) についての詳細をご覧ください。

**共有招待状:**

- [B2B の外部コラボレーションを有効にしてゲストを招待できるユーザーを管理する](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [ユーザーに対する特定組織からの招待を許可またはブロックする](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

**許可された ID プロバイダーの構成:**

- [Google フェデレーション](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [直接フェデレーション](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [ワンタイム パスコード認証をメールで送信する](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
