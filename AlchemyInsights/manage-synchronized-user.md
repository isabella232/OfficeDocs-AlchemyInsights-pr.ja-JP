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
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36542001"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="086f2-102">プライマリ メール アドレスを設定できない、またはユーザーの属性を変更できない</span><span class="sxs-lookup"><span data-stu-id="086f2-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="086f2-103">ご使用の環境でディレクトリ同期が有効になっている場合、一部のユーザーまたはオブジェクトの属性は Microsoft 365 管理センターを使用して変更できません。</span><span class="sxs-lookup"><span data-stu-id="086f2-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="086f2-104">同期されたユーザーとすべての属性を完全に管理するには、ローカルの Active Directory ユーザーとグループの管理コンソール (adsiedit.msc) を使用します。</span><span class="sxs-lookup"><span data-stu-id="086f2-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="086f2-105">または、次の一般的な例のように、PowerShell を使用して同期されたユーザーの個別ユーザーや属性を変更することができます。</span><span class="sxs-lookup"><span data-stu-id="086f2-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="086f2-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="086f2-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="086f2-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "テスト ユーザー" -LastName "ユーザー" -Title "マネージャーManager" -Department "HR"</span><span class="sxs-lookup"><span data-stu-id="086f2-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="086f2-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="086f2-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>