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
# <a name="troubleshoot-seamless-single-sign-on-sso-browser-issues"></a><span data-ttu-id="d2a8c-102">シームレス シングル サインオン (SSO) ブラウザーの問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="d2a8c-102">Troubleshoot Seamless Single Sign-on (SSO) browser issues</span></span>

<span data-ttu-id="d2a8c-103">ほとんどのユーザーは、次の手順を使用してシームレス SSO ブラウザーの問題を解決できます。</span><span class="sxs-lookup"><span data-stu-id="d2a8c-103">Most users are able to resolve their Seamless SSO browser issue using the steps below:</span></span>

1. <span data-ttu-id="d2a8c-104">お使いのブラウザーが最新であることを確認します。</span><span class="sxs-lookup"><span data-stu-id="d2a8c-104">Make sure your browser is up-to-date.</span></span>
2. <span data-ttu-id="d2a8c-105">ブラウザーから Cookie を削除して無効な SSO セッションを削除し、再度ログインしてみます。</span><span class="sxs-lookup"><span data-stu-id="d2a8c-105">Delete cookies from your browser to remove an invalid SSO session and try logging in again.</span></span>
3. <span data-ttu-id="d2a8c-106">別のブラウザーを使用してログインしてみます。</span><span class="sxs-lookup"><span data-stu-id="d2a8c-106">Try logging in using a different browser.</span></span>

<span data-ttu-id="d2a8c-107">**ブラウザーの既知の問題**</span><span class="sxs-lookup"><span data-stu-id="d2a8c-107">**Known Browser Issues**</span></span>

- <span data-ttu-id="d2a8c-108">シームレス SSO は、Firefox のプライベート ブラウズ モードでは動作しません。</span><span class="sxs-lookup"><span data-stu-id="d2a8c-108">Seamless SSO doesn't work in private browsing mode on Firefox.</span></span>
- <span data-ttu-id="d2a8c-109">拡張保護モードをオンにすると、Internet Explorer でシームレス SSO が動作しません。</span><span class="sxs-lookup"><span data-stu-id="d2a8c-109">Seamless SSO doesn't work in Internet Explorer when Enhanced Protected mode is turned on.</span></span>
- <span data-ttu-id="d2a8c-110">シームレス SSO は、Microsoft Edge (従来版) のプライベート ブラウズ モードでは動作しません。</span><span class="sxs-lookup"><span data-stu-id="d2a8c-110">Seamless SSO doesn't work in private browsing mode on Microsoft Edge (legacy).</span></span>
- <span data-ttu-id="d2a8c-111">シームレス SSO は、iOS および Android のモバイル ブラウザーでは動作しません。</span><span class="sxs-lookup"><span data-stu-id="d2a8c-111">Seamless SSO doesn't work on mobile browsers on iOS and Android.</span></span>

<span data-ttu-id="d2a8c-112">シームレス SSO は、Chromium ベースの次のバージョンの Microsoft Edge をサポートし、設計上、InPrivate モードとゲスト モードで動作します。</span><span class="sxs-lookup"><span data-stu-id="d2a8c-112">Seamless SSO supports the next version of Microsoft Edge based on Chromium and it works in InPrivate and Guest mode by design.</span></span>

<span data-ttu-id="d2a8c-113">**アドバイザリ**</span><span class="sxs-lookup"><span data-stu-id="d2a8c-113">**Advisory**</span></span>

<span data-ttu-id="d2a8c-114">シームレス SSO に関する機能要求または技術的な質問については、[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d2a8c-114">To make feature requests or ask technical questions about Seamless SSO, see [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html)</span></span>
