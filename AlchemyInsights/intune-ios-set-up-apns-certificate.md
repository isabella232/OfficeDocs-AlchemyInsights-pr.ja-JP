---
title: Intune iOS で APNS 証明書を設定する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "3543"
ms.openlocfilehash: f58405de018c916e08672022bb4f66292524b736
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667451"
---
# <a name="intune-ios-set-up-apns-certificate"></a><span data-ttu-id="b7b92-102">Intune iOS で APNS 証明書を設定する</span><span class="sxs-lookup"><span data-stu-id="b7b92-102">Intune iOS set up APNS certificate</span></span>

<span data-ttu-id="b7b92-103">Apple MDM プッシュ証明書 (Apple Push Notification Service (APNS) 証明書とも呼ばれます) が、お客様のサブスクリプションに構成されていません。</span><span class="sxs-lookup"><span data-stu-id="b7b92-103">An Apple MDM Push certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured on your subscription.</span></span>

<span data-ttu-id="b7b92-104">Apple MDM プッシュ証明書が構成されていないと、iOS デバイスや MacOS デバイスの登録および管理は行えません。</span><span class="sxs-lookup"><span data-stu-id="b7b92-104">Without an Apple MDM Push certificate configured, you'll be unable to enroll and manage iOS and MacOS devices.</span></span> <span data-ttu-id="b7b92-105">Intune に証明書を追加すると、ユーザーはポータル サイト アプリをインストールして iOS デバイスを登録することができるようになります。</span><span class="sxs-lookup"><span data-stu-id="b7b92-105">After you add the certificate to Intune, your users can install the Company Portal app to enroll their iOS devices.</span></span>

<span data-ttu-id="b7b92-106">Intune テナントに APNS 証明書を追加するためのステップ バイ ステップ ガイドについては、次のリンクのコンテンツを参照してください。</span><span class="sxs-lookup"><span data-stu-id="b7b92-106">For a step-by-step guide to adding an APNS certificate to your Intune tenant, please review the content on the following link:</span></span>

- [<span data-ttu-id="b7b92-107">Apple MDM プッシュ証明書を取得する</span><span class="sxs-lookup"><span data-stu-id="b7b92-107">Get an Apple MDM Push certificate</span></span>](https://docs.microsoft.com/mem/intune/enrollment/apple-mdm-push-certificate-get)

<span data-ttu-id="b7b92-108">Apple プッシュ通知証明書 (APN) に関する問題が発生している場合は、ブログ記事の「[Intune および APNs 証明書: FAQ と一般的な問題](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Intune-and-the-APNs-certificate-FAQ-and-common-issues/ba-p/280121)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b7b92-108">If you are having issues with the Apple Push Notification certificate (APNs) refer to this blog post: [Intune and the APNs certificate: FAQ and common issues](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Intune-and-the-APNs-certificate-FAQ-and-common-issues/ba-p/280121)</span></span>
