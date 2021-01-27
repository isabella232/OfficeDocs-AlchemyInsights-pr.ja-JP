---
title: SCIM プロビジョニングに関する問題
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
- "7854"
- "9004348"
ms.openlocfilehash: aa5b4cbb99cb1a5a323b39101766bea55fd49064
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/22/2021
ms.locfileid: "49950159"
---
# <a name="scim-provisioning-issue"></a><span data-ttu-id="eb241-102">SCIM プロビジョニングに関する問題</span><span class="sxs-lookup"><span data-stu-id="eb241-102">SCIM provisioning issue</span></span>

<span data-ttu-id="eb241-103">自動プロビジョニングとは、ユーザーがアクセスする必要のあるクラウド アプリケーションでユーザー ID と役割を作成することです。</span><span class="sxs-lookup"><span data-stu-id="eb241-103">Automatic provisioning refers to creating user identities and roles in the cloud applications that users need access to.</span></span> <span data-ttu-id="eb241-104">自動プロビジョニングには、ユーザー ID の作成に加えて、状態または役割の変更に伴うユーザー ID のメンテナンスおよび削除が含まれます。</span><span class="sxs-lookup"><span data-stu-id="eb241-104">In addition to creating user identities, automatic provisioning includes the maintenance and removal of user identities as status or roles change.</span></span> <span data-ttu-id="eb241-105">展開を開始する前に、[プロビジョニングの仕組み](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works)を確認して、Azure Active Directory (AD) プロビジョニングの仕組みを確認し、構成の推奨事項を取得できます。</span><span class="sxs-lookup"><span data-stu-id="eb241-105">Before you start a deployment, you can review [How provisioning works](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) to learn how Azure Active Directory (AD) provision works, and get configuration recommendations.</span></span>

<span data-ttu-id="eb241-106">アプリケーション開発者は、System for Cross-Domains Identity Management (SCIM) ユーザー管理 API を使用して、アプリケーションと Azure AD の間でユーザーとグループの自動プロビジョニングを有効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="eb241-106">As an application developer, you can use the System for Cross-Domain Identity Management (SCIM) user management API to enable automatic provisioning of users and groups between your application and Azure AD.</span></span> <span data-ttu-id="eb241-107">「[SCIM エンドポイントを構築し、Azure AD を使用してユーザー プロビジョニングを構成する](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups)」記事では、SCIM エンドポイントを構築して Azure AD プロビジョニング サービスと統合する方法について説明しています。</span><span class="sxs-lookup"><span data-stu-id="eb241-107">The [Build a SCIM endpoint and configure user provisioning with Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) article describes how to build an SCIM endpoint and integrate it with the Azure AD provisioning service.</span></span>



