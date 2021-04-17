---
title: Intune iOS で APNS 証明書を設定する
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "3543"
ms.openlocfilehash: 66590b8a063e74e80bbe3e1e497c596d63a54ece
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824044"
---
# <a name="intune-ios-set-up-apns-certificate"></a><span data-ttu-id="ce58d-102">Intune iOS で APNS 証明書を設定する</span><span class="sxs-lookup"><span data-stu-id="ce58d-102">Intune iOS set up APNS certificate</span></span>

<span data-ttu-id="ce58d-103">Apple MDM プッシュ証明書 (Apple Push Notification Service (APNS) 証明書とも呼ばれます) が、お客様のサブスクリプションに構成されていません。</span><span class="sxs-lookup"><span data-stu-id="ce58d-103">An Apple MDM Push certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured on your subscription.</span></span>

<span data-ttu-id="ce58d-104">Apple MDM プッシュ証明書が構成されていないと、iOS デバイスや MacOS デバイスの登録および管理は行えません。</span><span class="sxs-lookup"><span data-stu-id="ce58d-104">Without an Apple MDM Push certificate configured, you'll be unable to enroll and manage iOS and MacOS devices.</span></span> <span data-ttu-id="ce58d-105">Intune に証明書を追加すると、ユーザーはポータル サイト アプリをインストールして iOS デバイスを登録することができるようになります。</span><span class="sxs-lookup"><span data-stu-id="ce58d-105">After you add the certificate to Intune, your users can install the Company Portal app to enroll their iOS devices.</span></span>

<span data-ttu-id="ce58d-106">Intune テナントに APNS 証明書を追加するためのステップ バイ ステップ ガイドについては、次のリンクのコンテンツを参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce58d-106">For a step-by-step guide to adding an APNS certificate to your Intune tenant, please review the content on the following link:</span></span>

- [<span data-ttu-id="ce58d-107">Apple MDM プッシュ証明書を取得する</span><span class="sxs-lookup"><span data-stu-id="ce58d-107">Get an Apple MDM Push certificate</span></span>](https://docs.microsoft.com/mem/intune/enrollment/apple-mdm-push-certificate-get)

<span data-ttu-id="ce58d-108">Apple プッシュ通知証明書 (APN) に関する問題が発生している場合は、ブログ記事の「[Intune および APNs 証明書: FAQ と一般的な問題](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Intune-and-the-APNs-certificate-FAQ-and-common-issues/ba-p/280121)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce58d-108">If you are having issues with the Apple Push Notification certificate (APNs) refer to this blog post: [Intune and the APNs certificate: FAQ and common issues](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Intune-and-the-APNs-certificate-FAQ-and-common-issues/ba-p/280121)</span></span>
