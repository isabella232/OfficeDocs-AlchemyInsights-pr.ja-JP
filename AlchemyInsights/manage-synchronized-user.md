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
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380510"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>プライマリ メール アドレスを設定できない、またはユーザーの属性を変更できない

ご使用の環境でディレクトリ同期が有効になっている場合、一部のユーザーまたはオブジェクトの属性は管理センターを使用して変更できません。
同期されたユーザーとすべての属性を完全に管理するには、ローカルの Active Directory ユーザーとグループの管理コンソール (adsiedit.msc) を使用します。  

または、次の一般的な例のように、PowerShell を使用して同期されたユーザーの個別ユーザーや属性を変更することができます。 
- Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "テスト ユーザー" -LastName "ユーザー" -Title "マネージャーManager" -Department "HR"
- Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com