---
title: 自動で Microsoft Edge にサインインする
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/08/2020
ms.locfileid: "49680449"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="bd396-102">自動で Microsoft Edge にサインインする</span><span class="sxs-lookup"><span data-stu-id="bd396-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="bd396-103">Microsoft Edge は、OS の既定のアカウントを使用して、ユーザーのデバイス構成に従ってユーザーを自動的にサインインします。</span><span class="sxs-lookup"><span data-stu-id="bd396-103">Microsoft Edge uses the OS's default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="bd396-104">次に、各種類のデバイス構成とそれに依存するユーザー サインイン プロセスのシナリオを以下に説明します。</span><span class="sxs-lookup"><span data-stu-id="bd396-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

1. <span data-ttu-id="bd396-105">**デバイスがハイブリッド/AAD-J の場合**: このオプションは、Windows 10、下位レベルの Windows、および対応するサーバー バージョンで使用できます。</span><span class="sxs-lookup"><span data-stu-id="bd396-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="bd396-106">ユーザーは、Azure Active Directory (AD) アカウントで自動的にサインインします。</span><span class="sxs-lookup"><span data-stu-id="bd396-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
2. <span data-ttu-id="bd396-107">**デバイスがドメインに参加している場合**: このオプションは、Windows 10、下位レベルの Windows、および対応するサーバー バージョンで使用できます。</span><span class="sxs-lookup"><span data-stu-id="bd396-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="bd396-108">既定では、ドメイン アカウントを持つユーザーは自動的にサインインされません。ユーザーの自動サインインを有効にするには、**ConfigureOnPremisesAccountAutoSignIn** ポリシーを使用します。</span><span class="sxs-lookup"><span data-stu-id="bd396-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="bd396-109">Azure AD アカウントを持つユーザーの自動サインインを有効にするには、そのユーザーのデバイスにハイブリッド加入することを検討します。</span><span class="sxs-lookup"><span data-stu-id="bd396-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
3. <span data-ttu-id="bd396-110">**OS の既定のアカウントが Microsoft アカウントである場合**: このオプションは、Windows 10 RS3 (バージョン 1709、ビルド 10.0.16299) 以降のバージョンで使用できます。</span><span class="sxs-lookup"><span data-stu-id="bd396-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="bd396-111">このシナリオは、エンタープライズ デバイスではほとんど発生しません。</span><span class="sxs-lookup"><span data-stu-id="bd396-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="bd396-112">ただし、OS の既定のアカウントが Microsoft アカウントの場合、Microsoft Edge は自動的に Microsoft アカウントでユーザーをサインインします。</span><span class="sxs-lookup"><span data-stu-id="bd396-112">However, if the OS's default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
