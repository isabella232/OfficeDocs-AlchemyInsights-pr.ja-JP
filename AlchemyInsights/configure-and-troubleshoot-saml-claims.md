---
title: SAML クレームの構成とトラブルシューティング
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7799"
- "9004356"
ms.openlocfilehash: 306d2f451856a66f06447e3acd73e065da71cd64
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901718"
---
# <a name="configure-and-troubleshoot-saml-claims"></a><span data-ttu-id="ae4e8-102">SAML クレームの構成とトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="ae4e8-102">Configure and troubleshoot SAML claims</span></span>

<span data-ttu-id="ae4e8-103">SAML クレームの構成とトラブルシューティングを行うには:</span><span class="sxs-lookup"><span data-stu-id="ae4e8-103">To configure and troubleshoot SAML claims:</span></span>

1. <span data-ttu-id="ae4e8-104">[この記事](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management)で概説されている手順に従って、エンタープライズ アプリケーションのSAMLトークンで発行されるロールクレームを構成します。</span><span class="sxs-lookup"><span data-stu-id="ae4e8-104">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) to configure the role claim issued in the SAML token for enterprise applications.</span></span>
2. <span data-ttu-id="ae4e8-105">[この記事](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)の手順に従って、エンタープライズ アプリケーションの SAML トークンで発行されるクレームをカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="ae4e8-105">Follow the steps in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization) to customize claims issued in the SAML token for enterprise applications.</span></span>
3. <span data-ttu-id="ae4e8-106">[この記事](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)の手順に従って、テナント内の特定のアプリのトークンで発行されるクレームをカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="ae4e8-106">Follow the steps in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping) to customize claims emitted in tokens for a specific app in a tenant.</span></span>
4. <span data-ttu-id="ae4e8-107">[この記事](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications)を読んで、Application Proxy でのクレーム対応アプリの操作を理解してください。</span><span class="sxs-lookup"><span data-stu-id="ae4e8-107">Read [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications) to understand working with claims-aware apps in Application Proxy.</span></span>