---
title: 同期されたユーザーを管理する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380510"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="830cd-102">プライマリ電子メールアドレスを設定できない、またはユーザーの属性を変更できない</span><span class="sxs-lookup"><span data-stu-id="830cd-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="830cd-103">環境に対してディレクトリ同期が有効になっている場合は、管理センターを使用してユーザーまたはオブジェクトの属性を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="830cd-103">If directory synchronization is enabled for your environment some user or object attributes cannot be changed using the Admin Center.</span></span>
<span data-ttu-id="830cd-104">同期されたユーザーとそのすべての属性を完全に管理するには、ローカルの active directory ユーザーとグループ管理コンソール (adsiedit) を使用します。</span><span class="sxs-lookup"><span data-stu-id="830cd-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="830cd-105">または、次の一般的な例に示すように、個別のユーザーまたは属性を powershell を使用して変更することもできます。</span><span class="sxs-lookup"><span data-stu-id="830cd-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="830cd-106">Get-msoluser-UserPrincipalName user@yourdomain.onmicrosoft.com-AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="830cd-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="830cd-107">Get-msoluser-UserPrincipalName "user@yourdomain.onmicrosoft.com"-DisplayName "Test User"-LastName "User"-Title "Manager"-Department "HR"</span><span class="sxs-lookup"><span data-stu-id="830cd-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="830cd-108">Get-msoluser-UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="830cd-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>