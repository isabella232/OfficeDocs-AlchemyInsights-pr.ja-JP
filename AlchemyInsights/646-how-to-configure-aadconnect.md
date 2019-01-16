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
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28297326"
---
# <a name="configure-sync-features"></a><span data-ttu-id="3fe0c-102">同期機能を構成します。</span><span class="sxs-lookup"><span data-stu-id="3fe0c-102">Configure sync features</span></span>

<span data-ttu-id="3fe0c-p101">Azure AD 接続には、既定では、有効にするまたは後で有効にできるいくつかの機能が含まれています。いくつかの機能には、特定の環境に追加の構成が必要です。</span><span class="sxs-lookup"><span data-stu-id="3fe0c-p101">Azure AD Connect includes several features that are enabled by default, or that you can enable later. Some features require additional configuration in specific environments.</span></span>
  
- <span data-ttu-id="3fe0c-p102">[フィルタ リング](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering)の制限のオブジェクトは、Azure AD に同期されます。既定、すべてのユーザー、連絡先、グループ、および Windows の 10 では、コンピューター アカウントを同期します。ドメイン、Ou、またはその他の属性に基づいてオブジェクトを除外したりするできます。</span><span class="sxs-lookup"><span data-stu-id="3fe0c-p102">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD. By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized. You can include or exclude objects based on domains, OUs, or other attributes.</span></span> 
    
- <span data-ttu-id="3fe0c-p103">[パスワード ハッシュの同期](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization)は、パスワードのハッシュを Azure AD に、オンプレミスの Active directory を同期します。これにより、1 つの場所にパスワードの管理が、両方に同じパスワードを使用してオンプレミスおよびクラウド環境をします。Active Directory が権限のあるソースであるため、独自のパスワード ポリシーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="3fe0c-p103">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD. This allows password management in one location, but use of the same password in both on-premises and cloud environments. Because Active Directory is the authoritative source, you can use your own password policies.</span></span> 
    
- <span data-ttu-id="3fe0c-111">[セルフ サービスのパスワードのリセット (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr)も、オンプレミスのパスワード ポリシーの適用中に、雲の中、自分のパスワードをリセットできます。</span><span class="sxs-lookup"><span data-stu-id="3fe0c-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span> 
    
- <span data-ttu-id="3fe0c-112">[デバイスの書き戻し](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback)は、書き戻される、オンプレミスの Active Directory に条件付きのアクセスを使えるように Azure AD に登録されているデバイスを使用できます。</span><span class="sxs-lookup"><span data-stu-id="3fe0c-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span> 
    
- <span data-ttu-id="3fe0c-p104">[しない偶発的な削除](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes)は既定で有効に多数同時オブジェクトを削除 (同期あたり 500 個を超えるオブジェクト) を防ぐため。組織のニーズを満たすためには、この設定を変更することができます。</span><span class="sxs-lookup"><span data-stu-id="3fe0c-p104">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization). You can change this setting to meet the needs of your organization.</span></span> 
    
- <span data-ttu-id="3fe0c-115">高速インストールの既定[の自動アップグレード](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)が有効になっているし、Azure AD 接続のバージョンが現在では常にします。</span><span class="sxs-lookup"><span data-stu-id="3fe0c-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span> 
    

