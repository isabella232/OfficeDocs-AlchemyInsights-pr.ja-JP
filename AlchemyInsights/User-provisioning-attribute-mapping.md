---
title: ユーザー プロビジョニングの属性マッピング
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 73da476cc5913a16911839a59b80959d3c99a8bc22471febe421b022ce2c49ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918148"
---
# <a name="user-provisioning-attribute-mapping"></a>ユーザー プロビジョニングの属性マッピング

1. 既知の属性マッピングの問題のトラブルシューティングについては、「[属性マッピング](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings)」を参照してください。 
2. Microsoft Azure Active Directory (AD) は、Salesforce、G Suite などのサードパーティ製 SaaS アプリケーションへのユーザー プロビジョニングをサポートします。 サードパーティ製 SaaS アプリケーションのユーザー プロビジョニングを有効にすると、Azure portal は属性マッピングを介してその属性値を制御します。 既定の属性マッピングをカスタマイズする方法については、「[Azure Active Directory の SaaS アプリケーションのユーザー プロビジョニングの属性マッピングをカスタマイズする](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes)」を参照してください。
    - SaaS アプリのユーザー プロビジョニングの詳細については、「[Azure AD の自動化された SaaS アプリのユーザー プロビジョニングとは](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)」を参照してください。 
3. ユーザー プロビジョニング用に属性マッピングをカスタマイズする場合、マッピングする属性が [ソース属性] リストに表示されない場合があります。 「[アプリケーションにプロビジョニングするためにオンプレミスの Active Directory から Azure AD に属性を同期する](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping)」の記事では、オンプレミスの AD から Azure AD に同期することで、不足している属性を追加する方法を示しています。
