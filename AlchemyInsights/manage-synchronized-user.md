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
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>プライマリ電子メールアドレスを設定できない、またはユーザーの属性を変更できない

環境に対してディレクトリ同期が有効になっている場合、Microsoft 365 管理センターを使用して、一部のユーザー属性またはオブジェクト属性を変更することはできません。

同期されたユーザーとそのすべての属性を完全に管理するには、ローカルの active directory ユーザーとグループ管理コンソール (adsiedit) を使用します。  

または、次の一般的な例に示すように、個別のユーザーまたは属性を powershell を使用して変更することもできます。 
- Get-msoluser-UserPrincipalName user@yourdomain.onmicrosoft.com-AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Get-msoluser-UserPrincipalName "user@yourdomain.onmicrosoft.com"-DisplayName "Test User"-LastName "User"-Title "Manager"-Department "HR"
- Get-msoluser-UserPrincipalName "user@yourdomain.onmicrosoft.com