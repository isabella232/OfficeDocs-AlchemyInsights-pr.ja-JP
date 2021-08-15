---
title: プロビジョニング サービスの構成
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
- "9004687"
- "8468"
ms.openlocfilehash: 271ab7ad34c0f85f6f5a9d8d3dc2d901fe6fe8f978a2cc98eed986f594036f17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033283"
---
# <a name="configuring-the-provision-service"></a>プロビジョニング サービスの構成

自動化されたユーザー プロビジョニングを機能させるには、Azure AD が Workday Web Services API に接続できるようにする有効な資格情報が必要です。 さらに、Workday to AD ユーザーのプロビジョニング アプリの [接続テスト] ボタンは、AD ドメインに関連付けられた Azure AD Connect プロビジョニング エージェントに接続できるかどうかも検証します。

資格情報の保存時に Azure ポータルがエラーを返す場合は、以下の推奨手順に従ってください。

1. チュートリアル セクション「[Workday で統合システムユーザーを構成する](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)」の説明に従って、Workday 統合システム ユーザー アカウントを構成したことを確認します。
2. サービス管理コンソールを使用して、オンプレミスの Windows サーバーで Azure AD Connect プロビジョニング エージェント サービスが稼働していることを確認します。 [オンプレミス エージェントの表示] ボタンをクリックして、Azure ポータルでエージェントの状態を確認することもできます。
3. "Workday Username" フィールドの値を username@workday-tenant-name の形式で入力していることを確認してください。 workday-tenant-name が欠落している場合、Workday 認証は失敗します。
4. Workday 実装テナントとの統合を構成している場合は、Workday テナントのスケジュールされたダウンタイム時間をメモしてください。 Workday は、週末 (通常は金曜日の夜から土曜日の朝) に実装テナントのダウンタイムをスケジュールしており、このダウンタイム ウィンドウ中の接続障害は、実装テナントがオンラインに戻るとすぐに自動解決される既知の問題です。
5. まれに、テナントの更新のために統合システム ユーザーのパスワードが変更された場合、またはアカウントがロック状態または期限切れ状態にある場合にも、このエラーが表示されることがあります。 Integration System ユーザーのステータスを Workday 管理者に確認してください。

自動プロビジョニング用の Workday の構成の詳細については、「[チュートリアル: Workday を構成し、自動ユーザー プロビジョニングに対応させる](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)」を参照してください。
