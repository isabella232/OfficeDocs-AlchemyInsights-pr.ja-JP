---
title: Intune でカスタム通知を送信する
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886862"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="08a7a-102">管理対象の iOS および Android デバイスのユーザーにカスタム通知を送信する方法</span><span class="sxs-lookup"><span data-stu-id="08a7a-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="08a7a-103">Intuneのカスタム通知は、ユーザーのデバイスのポータル サイト アプリによって処理されます。</span><span class="sxs-lookup"><span data-stu-id="08a7a-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="08a7a-104">その後、アプリはそのデバイスでプッシュ通知を作成します。</span><span class="sxs-lookup"><span data-stu-id="08a7a-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="08a7a-105">カスタム通知の受信をサポートし、アプリがプッシュ通知を作成するためのデバイスの前提条件は以下のとおりです。</span><span class="sxs-lookup"><span data-stu-id="08a7a-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="08a7a-106">デバイスには、ポータル サイト アプリがインストールされている必要があります。</span><span class="sxs-lookup"><span data-stu-id="08a7a-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="08a7a-107">デバイスは、ポータル サイト アプリがプッシュ通知を送信できるようにしておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="08a7a-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="08a7a-108">アプリをインストールまたは更新すると、ユーザーに通知を許可するよう求めます。</span><span class="sxs-lookup"><span data-stu-id="08a7a-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="08a7a-109">Android デバイスには Google Play サービスがインストールされている必要があります。</span><span class="sxs-lookup"><span data-stu-id="08a7a-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="08a7a-110">デバイスを Intune に登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="08a7a-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="08a7a-111">メッセージの送信方法などの詳細については、[機能のドキュメント](https://docs.microsoft.com/intune/custom-notifications)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="08a7a-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
