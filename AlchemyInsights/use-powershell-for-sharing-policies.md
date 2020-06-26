---
title: PowerShell を使用してポリシーや組織の関係を共有する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862283"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="44700-102">PowerShell を使用してポリシーや組織の関係を共有する</span><span class="sxs-lookup"><span data-stu-id="44700-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="44700-103">組織の関係については、[Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation)、[New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship)、[Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)、[Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship) の詳細な構文とパラメーター情報をご確認ください。</span><span class="sxs-lookup"><span data-stu-id="44700-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="44700-104">共有ポリシーを作成するには、[New SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy) を使用します。</span><span class="sxs-lookup"><span data-stu-id="44700-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="44700-105">[メールボックスやユーザーに共有ポリシーを適用する](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)には、[Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) と [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) の組み合わせを新しく作成したポリシーとともに使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="44700-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="44700-106">[共有ポリシーを変更、無効化、削除する](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)には、[Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) と [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy) を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="44700-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="44700-107">**このトピックを完全に理解するためには、以下をお読みください。**</span><span class="sxs-lookup"><span data-stu-id="44700-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="44700-108">Exchange Online での共有</span><span class="sxs-lookup"><span data-stu-id="44700-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)