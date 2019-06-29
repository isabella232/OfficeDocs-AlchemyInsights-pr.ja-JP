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
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>プライマリ電子メールアドレスを設定できない、またはユーザーの属性を変更できない

環境に対してディレクトリ同期が有効になっている場合は、管理センターを使用してユーザーまたはオブジェクトの属性を変更することはできません。
同期されたユーザーとそのすべての属性を完全に管理するには、ローカルの active directory ユーザーとグループ管理コンソール (adsiedit) を使用します。  

または、次の一般的な例に示すように、個別のユーザーまたは属性を powershell を使用して変更することもできます。 
- Get-msoluser-UserPrincipalName user@yourdomain.onmicrosoft.com-AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Get-msoluser-UserPrincipalName "user@yourdomain.onmicrosoft.com"-DisplayName "Test User"-LastName "User"-Title "Manager"-Department "HR"
- Get-msoluser-UserPrincipalName "user@yourdomain.onmicrosoft.com