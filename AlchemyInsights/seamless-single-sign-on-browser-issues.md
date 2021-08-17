---
title: シームレス シングル サインオン (SSO) ブラウザーの問題のトラブルシューティング
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
- "9004357"
- "9377"
ms.openlocfilehash: f8617c15072f70778f7f4b151e75ffce4749f89ffa2b4d91730937c26aaeabbb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074289"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-browser-issues"></a>シームレス シングル サインオン (SSO) ブラウザーの問題のトラブルシューティング

ほとんどのユーザーは、次の手順を使用してシームレス SSO ブラウザーの問題を解決できます。

1. お使いのブラウザーが最新であることを確認します。
2. ブラウザーから Cookie を削除して無効な SSO セッションを削除し、再度ログインしてみます。
3. 別のブラウザーを使用してログインしてみます。

**ブラウザーの既知の問題**

- シームレス SSO は、Firefox のプライベート ブラウズ モードでは動作しません。
- 拡張保護モードをオンにすると、Internet Explorer でシームレス SSO が動作しません。
- シームレス SSO は、Microsoft Edge (従来版) のプライベート ブラウズ モードでは動作しません。
- シームレス SSO は、iOS および Android のモバイル ブラウザーでは動作しません。

シームレス SSO は、Chromium ベースの次のバージョンの Microsoft Edge をサポートし、設計上、InPrivate モードとゲスト モードで動作します。

**アドバイザリ**

シームレス SSO に関する機能要求または技術的な質問については、[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) を参照してください。
