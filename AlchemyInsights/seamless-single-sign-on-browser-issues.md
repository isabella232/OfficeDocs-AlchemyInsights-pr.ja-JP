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
ms.openlocfilehash: 507dc5a3bdc5f1bc27cf12865daf98df6c702827
ms.sourcegitcommit: f835aa80f2d85e9c0549be9395110377dba50f3d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2021
ms.locfileid: "50696474"
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
