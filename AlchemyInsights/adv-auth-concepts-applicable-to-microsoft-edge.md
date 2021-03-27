---
title: Microsoft Edge に適用できる高度な認証の概念
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398590"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Microsoft Edge に適用できる高度な認証の概念

Microsoft Edge に適用できる高度な認証の概念は次のとおりです。

**プロアクティブ認証**

[ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) ポリシーを有効にすると、Microsoft Edge はサインイン済みのユーザーのプロアクティブな認証を Microsoft サービス経由で試みます。 オンライン サービスを使用して、プロアクティブ認証を管理する構成を含むマニフェストの更新がないかどうかを定期的に確認します。

利点: プロアクティブ認証により、Office の新しいタブ ページなどの主要なサービスへの認証が有効になります。 さらに、検索エンジンに Bing が使われている場合、プロアクティブ認証によりアドレス バーのパフォーマンスが向上し、検索結果をビジネスのニーズに合わせてカスタマイズするのに役立ちます。

**Windows Hello CredUI for NTLM 認証**

Web サイトが NTLM またはネゴシエート メカニズムを通してユーザーのサインオンを試みたときにシングル サインオン (SSO) を利用できない場合、ユーザーはこの機能を使用して OS の資格情報を Web サイトと共有し、Windows Hello Cred UI を使用して認証の課題を満たすことができます。 このサインオン フローは、Windows 10 で NTLM またはネゴシエート チャレンジ中に SSO を取得できないユーザーにのみ表示されます。

**保存したパスワードを使用して自動的にサインオンする**

Microsoft Edge でパスワードを保存しているユーザーは、資格情報を保存した Web サイトへの自動サインオンを有効にすることができます。 ユーザーは edge://settings/passwords でこの機能のオンとオフを切り替えることができます。この機能は[パスワード マネージャー](https://go.microsoft.com/fwlink/?linkid=2134622) ポリシーで構成できます。
