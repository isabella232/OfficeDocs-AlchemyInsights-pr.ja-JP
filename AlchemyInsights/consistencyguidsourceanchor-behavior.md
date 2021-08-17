---
title: ConsistencyGuid/sourceAnchor の動作
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044345"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor の動作

Azure AD Connect (バージョン 1.1.524.0 以降) は、sourceAnchor 属性としての msDS-ConsistencyGuid の使用を容易にしました。この機能が使用されている場合は、Azure AD Connect が同期ルールを次のように自動的に構成します。
  
- ユーザー オブジェクトの sourceAnchor 属性として msDS-ConsistencyGuid を使用します。他のオブジェクトの種類では、ObjectGUID が使用されます。
    
- msDS-ConsistencyGuid 属性が入力されていない特定のオンプレミス AD ユーザー オブジェクトの場合は、Azure AD Connect がオンプレミス Active Directory 内の msDS-ConsistencyGuid 属性に objectGUID 値を書き戻します。msDS-ConsistencyGuid 属性が入力されると、Azure AD Connect が Azure AD にオブジェクトをエクスポートします。
    
 **メモ:** オンプレミス AD オブジェクトを Azure AD Connect にインポートする (つまり、AD コネクタ スペースにインポートしてから、Metaverse に投影する) と、sourceAnchor 値を変更できなくなります。特定のオンプレミス AD オブジェクトの SourceAnchor 値を指定するには、Azure AD Connect にインポートする前に、その msDS-ConsistencyGuid 属性を構成します。 
  
SourceAnchor と ConsistencyGuid の詳細については、「[Azure AD Connect: 設計概念](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)」を参照してください。
  

