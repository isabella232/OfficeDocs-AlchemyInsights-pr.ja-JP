---
title: 同期されたユーザーを管理する
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: bfa66492397adfd121fd3c9ddb2c190394cbc9a771a3e2c2db656ad438e404f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114783"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>プライマリ メール アドレスの設定、ユーザー属性の変更、または同期されたユーザーの削除はできません

ご使用の環境でディレクトリ同期が有効になっている場合、一部のユーザーまたはオブジェクトの属性は Microsoft 365 管理センターを使用して変更できません。

同期されたユーザーとすべての属性を完全に管理するには、ローカルの Active Directory ユーザーとグループの管理コンソール (adsiedit.msc) を使用します。  

または、次の一般的な例のように、PowerShell を使用して同期されたユーザーの個別ユーザーや属性を変更することができます。

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
