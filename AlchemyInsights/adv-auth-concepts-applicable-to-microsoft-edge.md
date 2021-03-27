---
title: Microsoft Edge に適用できる高度な認証の概念
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398590"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="86225-102">Microsoft Edge に適用できる高度な認証の概念</span><span class="sxs-lookup"><span data-stu-id="86225-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="86225-103">Microsoft Edge に適用できる高度な認証の概念は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="86225-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="86225-104">**プロアクティブ認証**</span><span class="sxs-lookup"><span data-stu-id="86225-104">**Proactive Authentication**</span></span>

<span data-ttu-id="86225-105">[ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) ポリシーを有効にすると、Microsoft Edge はサインイン済みのユーザーのプロアクティブな認証を Microsoft サービス経由で試みます。</span><span class="sxs-lookup"><span data-stu-id="86225-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="86225-106">オンライン サービスを使用して、プロアクティブ認証を管理する構成を含むマニフェストの更新がないかどうかを定期的に確認します。</span><span class="sxs-lookup"><span data-stu-id="86225-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="86225-107">利点: プロアクティブ認証により、Office の新しいタブ ページなどの主要なサービスへの認証が有効になります。</span><span class="sxs-lookup"><span data-stu-id="86225-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="86225-108">さらに、検索エンジンに Bing が使われている場合、プロアクティブ認証によりアドレス バーのパフォーマンスが向上し、検索結果をビジネスのニーズに合わせてカスタマイズするのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="86225-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="86225-109">**Windows Hello CredUI for NTLM 認証**</span><span class="sxs-lookup"><span data-stu-id="86225-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="86225-110">Web サイトが NTLM またはネゴシエート メカニズムを通してユーザーのサインオンを試みたときにシングル サインオン (SSO) を利用できない場合、ユーザーはこの機能を使用して OS の資格情報を Web サイトと共有し、Windows Hello Cred UI を使用して認証の課題を満たすことができます。</span><span class="sxs-lookup"><span data-stu-id="86225-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="86225-111">このサインオン フローは、Windows 10 で NTLM またはネゴシエート チャレンジ中に SSO を取得できないユーザーにのみ表示されます。</span><span class="sxs-lookup"><span data-stu-id="86225-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="86225-112">**保存したパスワードを使用して自動的にサインオンする**</span><span class="sxs-lookup"><span data-stu-id="86225-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="86225-113">Microsoft Edge でパスワードを保存しているユーザーは、資格情報を保存した Web サイトへの自動サインオンを有効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="86225-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="86225-114">ユーザーは edge://settings/passwords でこの機能のオンとオフを切り替えることができます。この機能は[パスワード マネージャー](https://go.microsoft.com/fwlink/?linkid=2134622) ポリシーで構成できます。</span><span class="sxs-lookup"><span data-stu-id="86225-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
