---
title: ConsistencyGuid/sourceAnchor の動作
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: cb1b50792b07a1b3b69607bf2f6824141a15922f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2019
ms.locfileid: "32408113"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor の動作

Azure AD Connect (バージョン 1.1.524.0 以降) は、sourceAnchor 属性としての msDS-ConsistencyGuid の使用を容易にしました。この機能が使用されている場合は、Azure AD Connect が同期ルールを次のように自動的に構成します。
  
- ユーザー オブジェクトの sourceAnchor 属性として msDS-ConsistencyGuid を使用します。他のオブジェクトの種類では、ObjectGUID が使用されます。
    
- msDS-ConsistencyGuid 属性が入力されていない特定のオンプレミス AD ユーザー オブジェクトの場合は、Azure AD Connect がオンプレミス Active Directory 内の msDS-ConsistencyGuid 属性に objectGUID 値を書き戻します。msDS-ConsistencyGuid 属性が入力されると、Azure AD Connect が Azure AD にオブジェクトをエクスポートします。
    
 **メモ:** オンプレミス AD オブジェクトを Azure AD Connect にインポートする (つまり、AD コネクタ スペースにインポートしてから、Metaverse に投影する) と、sourceAnchor 値を変更できなくなります。特定のオンプレミス AD オブジェクトの SourceAnchor 値を指定するには、Azure AD Connect にインポートする前に、その msDS-ConsistencyGuid 属性を構成します。 
  
SourceAnchor と ConsistencyGuid の詳細については、「[Azure AD Connect: 設計概念](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)」を参照してください。
  

