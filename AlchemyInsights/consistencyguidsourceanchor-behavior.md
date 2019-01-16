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
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28297423"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor の動作

Azure AD 接続 (バージョン 1.1.524.0 後と) msDS ConsistencyGuid の sourceAnchor の属性としての使用が容易になっています。この機能を使用すると、Azure AD 接続に同期規則が自動的に構成します。
  
- ユーザー オブジェクトの sourceAnchor 属性として msDS ConsistencyGuid を使用します。他のオブジェクト型のオブジェクト Guid が使用されます。
    
- 指定されたいずれかのオンプレミス AD ユーザー msDS ConsistencyGuid 属性を持つの objectGUID の値がバックアップ、オンプレミスの Active Directory で msDS ConsistencyGuid 属性に設定されている、Azure の AD 接続書き込みをされていないオブジェクトです。MsDS ConsistencyGuid 属性を読み込んだ後、Azure AD 接続は Azure AD にオブジェクトをエクスポートします。
    
 **注:** 1 回、オンプレミス AD オブジェクトは、Azure の AD 接続 (つまり、AD のコネクタ空間にインポートされ、メタバースに投影) にインポートは、もはや、sourceAnchor の値を変更することはできません。SourceAnchor 値を指定するのには、設置型を指定した AD オブジェクト、Azure AD 接続にインポートする前に、msDS ConsistencyGuid 属性を構成します。 
  
SourceAnchor と ConsistencyGuid の詳細については、以下を参照してください: [Azure AD 接続: 概念の設計](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

