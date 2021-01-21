---
title: ドメイン サービスの同期
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885814"
---
# <a name="domain-service-synchronization"></a>ドメイン サービスの同期

Azure Active Directory Domain Services (Azure AD DS) 管理ドメイン内のオブジェクトと資格情報は、ドメイン内でローカルに作成することも、Azure Active Directory (Azure AD) テナントから同期することもできます。 Azure AD DS を初めて展開するときは、自動一方向同期が構成され、Azure AD からオブジェクトを複製するように開始されます。 この一方向の同期はバックグラウンドで実行され続け、Azure AD DS 管理ドメインは Azure AD からの変更によって最新の状態に保たれます。 Azure AD DS から Azure AD への同期は行われません。

Azure Active Directory Domain Services の同期の詳細については、「[Domain Services の同期](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization)」を参照してください。 
