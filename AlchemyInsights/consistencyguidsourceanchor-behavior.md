---
title: ConsistencyGuid/sourceAnchor の動作
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 8527e7c2404742a999041f85ed12d78c48cc0d8c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705738"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="43930-102">ConsistencyGuid/sourceAnchor の動作</span><span class="sxs-lookup"><span data-stu-id="43930-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="43930-p101">Azure AD Connect (バージョン 1.1.524.0 以降) は、sourceAnchor 属性としての msDS-ConsistencyGuid の使用を容易にしました。この機能が使用されている場合は、Azure AD Connect が同期ルールを次のように自動的に構成します。</span><span class="sxs-lookup"><span data-stu-id="43930-p101">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute. When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="43930-p102">ユーザー オブジェクトの sourceAnchor 属性として msDS-ConsistencyGuid を使用します。他のオブジェクトの種類では、ObjectGUID が使用されます。</span><span class="sxs-lookup"><span data-stu-id="43930-p102">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects. ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="43930-p103">msDS-ConsistencyGuid 属性が入力されていない特定のオンプレミス AD ユーザー オブジェクトの場合は、Azure AD Connect がオンプレミス Active Directory 内の msDS-ConsistencyGuid 属性に objectGUID 値を書き戻します。msDS-ConsistencyGuid 属性が入力されると、Azure AD Connect が Azure AD にオブジェクトをエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="43930-p103">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory. After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="43930-p104">**メモ:** オンプレミス AD オブジェクトを Azure AD Connect にインポートする (つまり、AD コネクタ スペースにインポートしてから、Metaverse に投影する) と、sourceAnchor 値を変更できなくなります。特定のオンプレミス AD オブジェクトの SourceAnchor 値を指定するには、Azure AD Connect にインポートする前に、その msDS-ConsistencyGuid 属性を構成します。</span><span class="sxs-lookup"><span data-stu-id="43930-p104">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore. To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="43930-111">SourceAnchor と ConsistencyGuid の詳細については、「[Azure AD Connect: 設計概念](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="43930-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

