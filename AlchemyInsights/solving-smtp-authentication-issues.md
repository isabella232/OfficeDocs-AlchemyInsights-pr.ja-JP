---
title: SMTP 認証の問題を解決する
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
- "3000003"
- "5652"
ms.openlocfilehash: 3eaab2c601f78e20f2ee67bc21a9598cb45a24f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737994"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="13b7e-102">SMTP 認証の問題を解決する</span><span class="sxs-lookup"><span data-stu-id="13b7e-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="13b7e-103">SMTP メールを送信してクライアントまたはアプリケーションで認証しようとしたときにエラー 5.7.57 または 5.7.3 が発生した場合は、いくつかの点を確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="13b7e-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="13b7e-104">認証済みの SMTP 送信が、テナントまたは使用しようとしているメールボックスで無効になっている可能性があります (両方の設定を確認します)。</span><span class="sxs-lookup"><span data-stu-id="13b7e-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="13b7e-105">詳しくは、「[認証済みのクライアント SMTP 送信を有効または無効にする](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="13b7e-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="13b7e-106">テナントで [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) が有効になっているかどうかを確認します。有効になっていると、基本認証 (従来の認証とも呼ばれます。これはユーザー名とパスワードを使用します) を使用した SMTP 認証は失敗します。</span><span class="sxs-lookup"><span data-stu-id="13b7e-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
