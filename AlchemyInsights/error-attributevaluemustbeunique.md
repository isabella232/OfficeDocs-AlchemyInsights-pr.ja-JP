---
title: エラー AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7b98b68fabff6c048f1bab6cf506355114d18658
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916529"
---
# <a name="error-attributevaluemustbeunique"></a>エラー: AttributeValueMustBeUnique

AttributeValueMustBeUnique エラーの最も一般的な原因は、SourceAnchor (immutableId) が異なる 2 つのオブジェクトの ProxyAddresses 属性または UserPrincipalName 属性の値が同じであることです。AttributeValueMustBeUnique エラーを修正するには、次の手順を実行します。
  
1. エラーの原因になっている重複した proxyAddresses、userPrincipalName、またはその他の属性値を特定します。また、競合に関係している 2 つ以上のオブジェクトを特定します。Azure AD Connect Health for sync によって生成されるレポートが 2 つのオブジェクトの特定に役立ちます。
    
2. 重複した値を持ち続けるオブジェクトとそうでないオブジェクトを識別します。
    
3. 重複した値を持たないはずのオブジェクトから重複した値を除去します。オブジェクトの供給元になっているディレクトリで変更を加える必要があることに注意してください。競合しているオブジェクトのいずれかを削除しなければならない場合もあります。
    
4. オンプレミス AD で変更を加えた場合は、Azure AD Connect 同期にエラーを修正するための変更を指示します。
    

