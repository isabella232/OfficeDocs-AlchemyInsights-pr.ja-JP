---
title: 646 AADConnect の構成方法
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6cc4afb4b0f67fb76ecc7ff8f564b1cd36cc291c
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/22/2019
ms.locfileid: "31045139"
---
# <a name="configure-sync-features"></a><span data-ttu-id="f0fd2-102">同期機能を構成する</span><span class="sxs-lookup"><span data-stu-id="f0fd2-102">Configure sync features</span></span>

<span data-ttu-id="f0fd2-p101">Azure AD Connect には、既定で有効になる、または、後で有効にできるいくつかの機能が含まれています。環境によっては、機能に追加の構成が必要な場合があります。</span><span class="sxs-lookup"><span data-stu-id="f0fd2-p101">Azure AD Connect includes several features that are enabled by default, or that you can enable later. Some features require additional configuration in specific environments.</span></span>
  
- <span data-ttu-id="f0fd2-p102">[フィルター処理](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering)は、オブジェクトが Azure AD に同期されるように制限します。既定で、すべてのユーザー、連絡先、グループ、および Windows 10 コンピューター アカウントが同期されます。ドメイン、OU、またはその他の属性に基づいてオブジェクトを包含または除外できます。</span><span class="sxs-lookup"><span data-stu-id="f0fd2-p102">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD. By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized. You can include or exclude objects based on domains, OUs, or other attributes.</span></span> 
    
- <span data-ttu-id="f0fd2-p103">[パスワード ハッシュ同期](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization)は、パスワード ハッシュをオンプレミス Active Directory から Azure AD に同期します。これにより、1 か所でパスワードを管理し、オンプレミス環境とクラウド環境の両方で同じパスワードを使用できるようになります。Active Directory は権限を持っているソースのため、独自のパスワード ポリシーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="f0fd2-p103">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD. This allows password management in one location, but use of the same password in both on-premises and cloud environments. Because Active Directory is the authoritative source, you can use your own password policies.</span></span> 
    
- <span data-ttu-id="f0fd2-111">[セルフ サービスによるパスワードのリセット (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) を使用すれば、ユーザーは、オンプレミス パスワード ポリシーを適用しながら、クラウドで独自のパスワードをリセットすることができます。</span><span class="sxs-lookup"><span data-stu-id="f0fd2-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span> 
    
- <span data-ttu-id="f0fd2-112">[デバイスの書き戻し](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback)を使用すれば、Azure AD に登録されているデバイスをオンプレミス Active Directory に書き戻すことができるため、条件付きアクセスに使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="f0fd2-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span> 
    
- <span data-ttu-id="f0fd2-p104">[偶発的削除の防止](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes)は、同時オブジェクト削除が頻発 (同期あたり 500 を超えるオブジェクトの削除) しないように既定で有効になります。この設定は、組織のニーズに合わせて変更することができます。</span><span class="sxs-lookup"><span data-stu-id="f0fd2-p104">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization). You can change this setting to meet the needs of your organization.</span></span> 
    
- <span data-ttu-id="f0fd2-115">[自動アップグレード](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)は、高速インストール用に既定で有効になり、Azure AD Connect のバージョンが常に最新であることの保証を支援します。</span><span class="sxs-lookup"><span data-stu-id="f0fd2-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span> 
    

