---
title: 社内でのシームレス シングル サインオン (SSO) のトラブルシューティング
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9370"
- "9004357"
ms.openlocfilehash: a8d14b12bfb3b02da0468eee70af26344465a2a2
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816527"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-for-on-premises"></a><span data-ttu-id="f6ba4-102">社内でのシームレス シングル サインオン (SSO) のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="f6ba4-102">Troubleshoot Seamless Single Sign-on (SSO) for on-premises</span></span>

<span data-ttu-id="f6ba4-103">シングル サインオン (SSO) の問題を解決するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="f6ba4-103">To resolve Seamless Single Sign-on (SSO) issues, perform the following steps:</span></span>

<span data-ttu-id="f6ba4-104">**AZUREADSSO　コンピューター アカウントの Kerberos 復号化キーをロール オーバーする方法**</span><span class="sxs-lookup"><span data-stu-id="f6ba4-104">**How can I roll over the Kerberos decryption key of the AZUREADSSO computer account?**</span></span>

<span data-ttu-id="f6ba4-105">少なくとも 30 日ごとに Kerberos 復号化キーをロール オーバーすることを強くお勧めします。</span><span class="sxs-lookup"><span data-stu-id="f6ba4-105">We highly recommend that you roll over the Kerberos decryption key at least every 30 days.</span></span> <span data-ttu-id="f6ba4-106">これを手動で行うには、「[Kerberos 復号化キーをロール オーバーする方法](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f6ba4-106">To do this manually, see [How to roll over Kerberos decryption keys](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span></span>

<span data-ttu-id="f6ba4-107">**シームレスな SSO を構成する**</span><span class="sxs-lookup"><span data-stu-id="f6ba4-107">**Configure Seamless SSO**</span></span>

<span data-ttu-id="f6ba4-108">シームレスな SSO を展開するには、「[Azure Active Directory シームレス シングル サインオン: クイックスタート](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys)」の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="f6ba4-108">To deploy Seamless SSO, follow the steps in [Azure Active Directory Seamless Single Sign-On: Quickstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span></span>

<span data-ttu-id="f6ba4-109">**アドバイザリ**</span><span class="sxs-lookup"><span data-stu-id="f6ba4-109">**Advisory**</span></span>

- <span data-ttu-id="f6ba4-110">[Azure Active Directory シームレス シングル サインオン: よく寄せられる質問](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) - この記事では、Azure Active Directory シームレス シングル サインオン (Seamless SSO) に関するよくある質問をご紹介します。</span><span class="sxs-lookup"><span data-stu-id="f6ba4-110">[Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) - In this article, we address frequently asked questions about Azure Active Directory Seamless Single Sign-On (Seamless SSO).</span></span> <span data-ttu-id="f6ba4-111">新しいコンテンツをときどき確認してください。</span><span class="sxs-lookup"><span data-stu-id="f6ba4-111">Keep checking back for new content.</span></span>
- <span data-ttu-id="f6ba4-112">[Microsoft よく寄せられる質問](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - この記事では、シームレス シングル サインオンに関する機能の要求や技術的な質問する方法をご紹介します。</span><span class="sxs-lookup"><span data-stu-id="f6ba4-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - This article provides information on how to make feature requests or ask technical questions about Seamless SSO.</span></span>

<span data-ttu-id="f6ba4-113">**トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="f6ba4-113">**Troubleshoot**</span></span>

<span data-ttu-id="f6ba4-114">[Azure Active Directory のシームレス シングル サインオン](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) - この記事では、Azure Active Directory (Azure AD) のシームレス シングル サインオン (Seamless SSO) に関する一般的な問題について、トラブルシューティングに関する情報を確認できます。</span><span class="sxs-lookup"><span data-stu-id="f6ba4-114">[Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) - This article helps you find troubleshooting information about common problems regarding Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).</span></span>







