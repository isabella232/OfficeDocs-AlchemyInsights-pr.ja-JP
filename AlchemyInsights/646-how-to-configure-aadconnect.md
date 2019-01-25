---
title: 646 AADConnect を構成する方法
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: e4ba295cd0661c3454180dd6a15895123840389e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499675"
---
# <a name="configure-sync-features"></a>同期機能を構成します。

Azure AD 接続には、既定では、有効にするまたは後で有効にできるいくつかの機能が含まれています。いくつかの機能には、特定の環境に追加の構成が必要です。
  
- [フィルタ リング](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering)の制限のオブジェクトは、Azure AD に同期されます。既定、すべてのユーザー、連絡先、グループ、および Windows の 10 では、コンピューター アカウントを同期します。ドメイン、Ou、またはその他の属性に基づいてオブジェクトを除外したりするできます。 
    
- [パスワード ハッシュの同期](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization)は、パスワードのハッシュを Azure AD に、オンプレミスの Active directory を同期します。これにより、1 つの場所にパスワードの管理が、両方に同じパスワードを使用してオンプレミスおよびクラウド環境をします。Active Directory が権限のあるソースであるため、独自のパスワード ポリシーを使用できます。 
    
- [セルフ サービスのパスワードのリセット (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr)も、オンプレミスのパスワード ポリシーの適用中に、雲の中、自分のパスワードをリセットできます。 
    
- [デバイスの書き戻し](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback)は、書き戻される、オンプレミスの Active Directory に条件付きのアクセスを使えるように Azure AD に登録されているデバイスを使用できます。 
    
- [しない偶発的な削除](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes)は既定で有効に多数同時オブジェクトを削除 (同期あたり 500 個を超えるオブジェクト) を防ぐため。組織のニーズを満たすためには、この設定を変更することができます。 
    
- 高速インストールの既定[の自動アップグレード](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)が有効になっているし、Azure AD 接続のバージョンが現在では常にします。 
    

