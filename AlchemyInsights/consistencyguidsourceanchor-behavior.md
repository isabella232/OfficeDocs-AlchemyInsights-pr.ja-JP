---
title: ConsistencyGuid/sourceAnchor の動作
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 010474bcc4cc6f97bcaafef9dfe6f4accfed4247
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29659596"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor の動作

Azure AD Connect (バージョン 1.1.524.0 以降) は、sourceAnchor 属性としての msDS-ConsistencyGuid の使用を容易にしました。この機能が使用されている場合は、Azure AD Connect が同期ルールを次のように自動的に構成します。
  
- ユーザー オブジェクトの sourceAnchor 属性として msDS-ConsistencyGuid を使用します。他のオブジェクトの種類では、ObjectGUID が使用されます。
    
- msDS-ConsistencyGuid 属性が入力されていない特定のオンプレミス AD ユーザー オブジェクトの場合は、Azure AD Connect がオンプレミス Active Directory 内の msDS-ConsistencyGuid 属性に objectGUID 値を書き戻します。msDS-ConsistencyGuid 属性が入力されると、Azure AD Connect が Azure AD にオブジェクトをエクスポートします。
    
 **メモ:** オンプレミス AD オブジェクトを Azure AD Connect にインポートする (つまり、AD コネクタ スペースにインポートしてから、Metaverse に投影する) と、sourceAnchor 値を変更できなくなります。特定のオンプレミス AD オブジェクトの SourceAnchor 値を指定するには、Azure AD Connect にインポートする前に、その msDS-ConsistencyGuid 属性を構成します。 
  
SourceAnchor と ConsistencyGuid の詳細については、「[Azure AD Connect: 設計概念](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)」を参照してください。
  

