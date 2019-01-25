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
ms.openlocfilehash: 80516ed9e15040475a8b65a1af98a1b561704d49
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29498523"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="c8410-102">ConsistencyGuid/sourceAnchor の動作</span><span class="sxs-lookup"><span data-stu-id="c8410-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="c8410-p101">Azure AD 接続 (バージョン 1.1.524.0 後と) msDS ConsistencyGuid の sourceAnchor の属性としての使用が容易になっています。この機能を使用すると、Azure AD 接続に同期規則が自動的に構成します。</span><span class="sxs-lookup"><span data-stu-id="c8410-p101">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute. When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="c8410-p102">ユーザー オブジェクトの sourceAnchor 属性として msDS ConsistencyGuid を使用します。他のオブジェクト型のオブジェクト Guid が使用されます。</span><span class="sxs-lookup"><span data-stu-id="c8410-p102">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects. ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="c8410-p103">指定されたいずれかのオンプレミス AD ユーザー msDS ConsistencyGuid 属性を持つの objectGUID の値がバックアップ、オンプレミスの Active Directory で msDS ConsistencyGuid 属性に設定されている、Azure の AD 接続書き込みをされていないオブジェクトです。MsDS ConsistencyGuid 属性を読み込んだ後、Azure AD 接続は Azure AD にオブジェクトをエクスポートします。</span><span class="sxs-lookup"><span data-stu-id="c8410-p103">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory. After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="c8410-p104">**注:** 1 回、オンプレミス AD オブジェクトは、Azure の AD 接続 (つまり、AD のコネクタ空間にインポートされ、メタバースに投影) にインポートは、もはや、sourceAnchor の値を変更することはできません。SourceAnchor 値を指定するのには、設置型を指定した AD オブジェクト、Azure AD 接続にインポートする前に、msDS ConsistencyGuid 属性を構成します。</span><span class="sxs-lookup"><span data-stu-id="c8410-p104">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore. To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="c8410-111">SourceAnchor と ConsistencyGuid の詳細については、以下を参照してください: [Azure AD 接続: 概念の設計](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="c8410-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

