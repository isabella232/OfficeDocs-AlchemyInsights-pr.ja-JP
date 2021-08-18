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
ms.openlocfilehash: 58acaa29f9d0b066cc7be6f6ee57b1806d0e8812b194e20166b133b7715226a8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086169"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>管理対象の iOS および Android デバイスのユーザーにカスタム通知を送信する方法

Intuneのカスタム通知は、ユーザーのデバイスのポータル サイト アプリによって処理されます。 その後、アプリはそのデバイスでプッシュ通知を作成します。

カスタム通知の受信をサポートし、アプリがプッシュ通知を作成するためのデバイスの前提条件は以下のとおりです。

- デバイスには、ポータル サイト アプリがインストールされている必要があります。  

- デバイスは、ポータル サイト アプリがプッシュ通知を送信できるようにしておく必要があります。 アプリをインストールまたは更新すると、ユーザーに通知を許可するよう求めます。

- Android デバイスには Google Play サービスがインストールされている必要があります。

- デバイスを Intune に登録する必要があります。

メッセージの送信方法などの詳細については、[機能のドキュメント](https://docs.microsoft.com/intune/custom-notifications)を参照してください。
