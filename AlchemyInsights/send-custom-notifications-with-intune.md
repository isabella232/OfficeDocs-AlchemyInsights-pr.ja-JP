---
title: Intune でカスタム通知を送信する
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/16/2019
ms.locfileid: "37023556"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a>管理対象の iOS および Android デバイスのユーザーにカスタム通知を送信する方法

Intuneのカスタム通知は、ユーザーのデバイスのポータル サイト アプリによって処理されます。 その後、アプリはそのデバイスでプッシュ通知を作成します。

カスタム通知の受信をサポートし、アプリがプッシュ通知を作成するためのデバイスの前提条件は以下のとおりです。

- デバイスには、ポータル サイト アプリがインストールされている必要があります。  

- デバイスは、ポータル サイト アプリがプッシュ通知を送信できるようにしておく必要があります。 アプリをインストールまたは更新すると、ユーザーに通知を許可するよう求めます。

- Android デバイスには Google Play サービスがインストールされている必要があります。

- デバイスを Intune に登録する必要があります。

メッセージの送信方法などの詳細については、[機能のドキュメント](https://docs.microsoft.com/intune/custom-notifications)を参照してください。
