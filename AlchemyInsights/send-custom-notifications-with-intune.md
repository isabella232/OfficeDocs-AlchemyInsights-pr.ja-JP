---
title: Intune でカスタム通知を送信する
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720651"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>管理対象の iOS および Android デバイスのユーザーにカスタム通知を送信する方法

Intuneのカスタム通知は、ユーザーのデバイスのポータル サイト アプリによって処理されます。 その後、アプリはそのデバイスでプッシュ通知を作成します。

カスタム通知の受信をサポートし、アプリがプッシュ通知を作成するためのデバイスの前提条件は以下のとおりです。

- デバイスには、ポータル サイト アプリがインストールされている必要があります。  

- デバイスは、ポータル サイト アプリがプッシュ通知を送信できるようにしておく必要があります。 アプリをインストールまたは更新すると、ユーザーに通知を許可するよう求めます。

- Android デバイスには Google Play サービスがインストールされている必要があります。

- デバイスを Intune に登録する必要があります。

メッセージの送信方法などの詳細については、[機能のドキュメント](https://docs.microsoft.com/intune/custom-notifications)を参照してください。
