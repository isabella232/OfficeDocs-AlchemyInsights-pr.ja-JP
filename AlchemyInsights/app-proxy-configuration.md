---
title: アプリ プロキシの構成
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885811"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="772e1-102">アプリ プロキシの構成</span><span class="sxs-lookup"><span data-stu-id="772e1-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="772e1-103">オンプレミス アプリケーションをクラウドに公開するように Azure AD 内でアプリケーション プロキシ アプリケーションを設定する方法については、「[アプリケーション プロキシ アプリケーションの構成方法](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="772e1-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="772e1-104">シングル サインオン (SSO) を使用すると、ユーザーは複数回認証しなくてもアプリケーションにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="772e1-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="772e1-105">これにより、Azure Active Directory に対してクラウド上で単一の認証を行うことができ、サービスまたはコネクタがユーザーになりすますことで、アプリケーションからの追加の認証確認を完了できます。</span><span class="sxs-lookup"><span data-stu-id="772e1-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="772e1-106">詳細については、「[アプリケーション プロキシ アプリケーションへのシングル サインオンの構成方法](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="772e1-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="772e1-107">[この記事](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem)を使用して、新しいアプリケーション プロキシ アプリケーションの作成時に発生する一般的な問題のトラブルシューティングを行ってください。</span><span class="sxs-lookup"><span data-stu-id="772e1-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="772e1-108">アプリケーションに対するバックエンド認証のセットアップで問題が発生した場合は、[アプリケーション プロキシの Kerberos 制約付き委任構成のトラブルシューティングを行う](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to)か、「[PingAccess を使用してアプリケーションを構成する](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to)」のガイダンスに従って問題を解決する必要があります。</span><span class="sxs-lookup"><span data-stu-id="772e1-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
