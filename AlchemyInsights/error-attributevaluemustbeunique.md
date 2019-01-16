---
title: エラー AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7a97d1a5ff352b55833bd457e3220a56130d7e7e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28297789"
---
# <a name="error-attributevaluemustbeunique"></a>エラー: AttributeValueMustBeUnique

AttributeValueMustBeUnique エラーの最も一般的な理由は、別の SourceAnchor (immutableId) と 2 つのオブジェクトが ProxyAddresses、UserPrincipalName 属性に同じ値を持ちます。AttributeValueMustBeUnique エラーを修正するには。
  
1. 重複 proxyAddresses、userPrincipalName またはエラーの原因となっている他の属性値を識別します。競合に関連する 2 つ (以上) のオブジェクトを識別します。Azure AD 接続の稼働状態の同期によって生成されるレポートは、2 つのオブジェクトを識別するのに役立ちます。
    
2. 重複した値を設定するオブジェクトを続行する必要がありますであり、どのオブジェクトを識別します。
    
3. オブジェクトをその値を持たないする必要がありますから、重複した値を削除します。オブジェクトを供給する場所のディレクトリに変更を行う必要があることに注意してください。場合によっては、競合しているオブジェクトの 1 つを削除する必要があります。
    
4. AD の施設内で変更を加えた場合は、Azure の AD 接続を修正するのにはエラーが発生する変更の同期を使用できます。
    

