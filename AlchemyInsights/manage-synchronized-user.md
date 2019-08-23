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
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36542001"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="7bec8-102">プライマリ電子メールアドレスを設定できない、またはユーザーの属性を変更できない</span><span class="sxs-lookup"><span data-stu-id="7bec8-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="7bec8-103">環境に対してディレクトリ同期が有効になっている場合、Microsoft 365 管理センターを使用して、一部のユーザー属性またはオブジェクト属性を変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="7bec8-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="7bec8-104">同期されたユーザーとそのすべての属性を完全に管理するには、ローカルの active directory ユーザーとグループ管理コンソール (adsiedit) を使用します。</span><span class="sxs-lookup"><span data-stu-id="7bec8-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="7bec8-105">または、次の一般的な例に示すように、個別のユーザーまたは属性を powershell を使用して変更することもできます。</span><span class="sxs-lookup"><span data-stu-id="7bec8-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="7bec8-106">Get-msoluser-UserPrincipalName user@yourdomain.onmicrosoft.com-AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="7bec8-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="7bec8-107">Get-msoluser-UserPrincipalName "user@yourdomain.onmicrosoft.com"-DisplayName "Test User"-LastName "User"-Title "Manager"-Department "HR"</span><span class="sxs-lookup"><span data-stu-id="7bec8-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="7bec8-108">Get-msoluser-UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="7bec8-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>