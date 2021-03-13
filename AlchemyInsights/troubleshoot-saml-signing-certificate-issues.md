---
title: SAML 署名による証明書の問題のトラブルシューティング
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2021
ms.locfileid: "50696402"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="80bdf-102">SAML 署名による証明書の問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="80bdf-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="80bdf-103">SAML 署名による証明書の問題を解決するには、次の推奨手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="80bdf-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="80bdf-104">SSO をサポートするエンタープライズ アプリケーションを追加すると、Azure は [SAML 署名による証明書](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications)と呼ばれる証明書を生成します。</span><span class="sxs-lookup"><span data-stu-id="80bdf-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="80bdf-105">この証明書の有効期限は 3 年です。</span><span class="sxs-lookup"><span data-stu-id="80bdf-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="80bdf-106">証明書の有効期限を変更するには、「 [フェデレーション証明書の有効期限をカスタマイズして、新しい証明書にロール オーバーする](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="80bdf-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="80bdf-107">Azure では、この証明書を使用して、アプリケーションから要求された SAML トークンに署名し、SSO を成功させるためにアプリケーションに送信します。</span><span class="sxs-lookup"><span data-stu-id="80bdf-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="80bdf-108">この手順を完了するには、Azure portal から証明書をダウンロードし、アプリケーション ベンダーに送信して SSO プロセスを完了します。</span><span class="sxs-lookup"><span data-stu-id="80bdf-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="80bdf-109">このプロセスが完了すると、アプリケーションはこの証明書を信頼し、この証明書によって署名された SAML トークンはすべてアプリケーションで承認されます。</span><span class="sxs-lookup"><span data-stu-id="80bdf-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="80bdf-110">この証明書の有効期限が切れた場合は、新しい証明書を作成し、アプリケーション ベンダーに更新してから、Azure 側でアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="80bdf-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="80bdf-111">詳細については、「[有効期限が切れそうな証明書を更新する](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="80bdf-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="80bdf-112">証明書の有効期限が切れた場合、ユーザーはブロックされません。</span><span class="sxs-lookup"><span data-stu-id="80bdf-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="80bdf-113">現在の証明書の有効期限が切れる前に、[通知を受信するための電子メールアドレスを追加](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration)します。</span><span class="sxs-lookup"><span data-stu-id="80bdf-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="80bdf-114">手順 4 は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="80bdf-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="80bdf-115">アプリケーションの SAML 証明書の署名オプションと証明書の署名アルゴリズムを変更します。</span><span class="sxs-lookup"><span data-stu-id="80bdf-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="80bdf-116">詳細については、「[証明書の署名オプションと署名アルゴリズムの変更](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="80bdf-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

