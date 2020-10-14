---
title: 同期されたユーザーを管理する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 7bf7d3f00308ff6bc973cd52e09ca51c5fd0f45b
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451405"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="9a304-102">プライマリ メール アドレスの設定、ユーザー属性の変更、または同期されたユーザーの削除はできません</span><span class="sxs-lookup"><span data-stu-id="9a304-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="9a304-103">ご使用の環境でディレクトリ同期が有効になっている場合、一部のユーザーまたはオブジェクトの属性は Microsoft 365 管理センターを使用して変更できません。</span><span class="sxs-lookup"><span data-stu-id="9a304-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="9a304-104">同期されたユーザーとすべての属性を完全に管理するには、ローカルの Active Directory ユーザーとグループの管理コンソール (adsiedit.msc) を使用します。</span><span class="sxs-lookup"><span data-stu-id="9a304-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="9a304-105">または、次の一般的な例のように、PowerShell を使用して同期されたユーザーの個別ユーザーや属性を変更することができます。</span><span class="sxs-lookup"><span data-stu-id="9a304-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span>

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
