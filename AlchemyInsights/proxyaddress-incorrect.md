---
title: メタベースが正しくありません。
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
ms.assetid: c4cea778-1b26-4aea-bde8-4b7605e35886
ms.openlocfilehash: e6af15bb29c6808acab3169ffbc5f4820e258a26
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29654492"
---
# <a name="proxyaddress-incorrect"></a><span data-ttu-id="81b4f-102">メタベースが正しくありません。</span><span class="sxs-lookup"><span data-stu-id="81b4f-102">ProxyAddress incorrect</span></span>

<span data-ttu-id="81b4f-p101">Azure AD にオブジェクトを同期すると、Azure AD 規則では、Active Directory の proxyAddresses 属性に指定されている値を比較し、Azure AD に proxyAddresses 属性を設定し、します。したがって、Active Directory 内のオブジェクトの proxyAddresses 属性の値は proxyAddresses 属性の値と同じでできません Azure AD。</span><span class="sxs-lookup"><span data-stu-id="81b4f-p101">When an object is synchronized to Azure AD, the values that are specified in the proxyAddresses attribute in Active Directory are compared with Azure AD rules, and then the proxyAddresses attribute is populated in Azure AD. Therefore, the values of the proxyAddresses attribute for the object in Active Directory may not be the same as the values of the proxyAddresses attribute in Azure AD.</span></span>
  
<span data-ttu-id="81b4f-105">メタベースの設定方法に関する詳細については、 [Azure AD でメタベースの属性を設定する方法](https://support.microsoft.com/help/3190357/how-the-proxyaddresses-attribute-is-populated-in-azure-ad)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="81b4f-105">To learn more about how the proxyaddress is populated, see [How the proxyAddress attribute is populated in Azure AD](https://support.microsoft.com/help/3190357/how-the-proxyaddresses-attribute-is-populated-in-azure-ad).</span></span>
  

