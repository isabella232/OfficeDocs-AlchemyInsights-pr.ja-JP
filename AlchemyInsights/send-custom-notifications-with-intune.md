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
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/16/2019
ms.locfileid: "37023556"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="7188d-102">管理対象 iOS および Android デバイスのユーザーにカスタム通知を送信する方法</span><span class="sxs-lookup"><span data-stu-id="7188d-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="7188d-103">Intune のカスタム通知は、ユーザーのデバイス上の会社のポータルアプリによって処理されます。</span><span class="sxs-lookup"><span data-stu-id="7188d-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="7188d-104">その後、アプリはそのデバイスでプッシュ通知を作成します。</span><span class="sxs-lookup"><span data-stu-id="7188d-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="7188d-105">カスタム通知の受信をサポートするためのデバイスの前提条件、およびアプリでプッシュ通知を作成する場合の前提条件を以下に示します。</span><span class="sxs-lookup"><span data-stu-id="7188d-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="7188d-106">デバイスには、会社のポータルアプリがインストールされている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7188d-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="7188d-107">デバイスでは、ポータルサイトアプリでプッシュ通知を送信できるようにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="7188d-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="7188d-108">アプリがインストールまたは更新されると、ユーザーに通知を許可するかどうかを確認するメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="7188d-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="7188d-109">Android デバイスには、Google Play サービスがインストールされている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7188d-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="7188d-110">デバイスを Intune に登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7188d-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="7188d-111">メッセージの送信方法などの詳細については、[機能のドキュメント](https://docs.microsoft.com/intune/custom-notifications)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7188d-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
