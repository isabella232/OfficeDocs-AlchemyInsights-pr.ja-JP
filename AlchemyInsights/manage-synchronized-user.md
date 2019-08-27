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
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>プライマリ メール アドレスを設定できない、またはユーザーの属性を変更できない

ご使用の環境でディレクトリ同期が有効になっている場合、一部のユーザーまたはオブジェクトの属性は Microsoft 365 管理センターを使用して変更できません。

同期されたユーザーとすべての属性を完全に管理するには、ローカルの Active Directory ユーザーとグループの管理コンソール (adsiedit.msc) を使用します。  

または、次の一般的な例のように、PowerShell を使用して同期されたユーザーの個別ユーザーや属性を変更することができます。 
- Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "テスト ユーザー" -LastName "ユーザー" -Title "マネージャーManager" -Department "HR"
- Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com