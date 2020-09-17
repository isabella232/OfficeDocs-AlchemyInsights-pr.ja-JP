---
title: PowerShell を使用してポリシーや組織の関係を共有する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 378dedb332ced2c86899401c54726eb6b7e25d08
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773420"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>PowerShell を使用してポリシーや組織の関係を共有する


組織の関係については、[Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation)、[New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship)、[Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)、[Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship) の詳細な構文とパラメーター情報をご確認ください。

共有ポリシーを作成するには、[New SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy) を使用します。 [メールボックスやユーザーに共有ポリシーを適用する](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)には、[Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) と [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) の組み合わせを新しく作成したポリシーとともに使用する必要があります。 [共有ポリシーを変更、無効化、削除する](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)には、[Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) と [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy) を使用する必要があります。

**このトピックを完全に理解するためには、以下をお読みください。**

[Exchange Online での共有](https://docs.microsoft.com/exchange/sharing/sharing)