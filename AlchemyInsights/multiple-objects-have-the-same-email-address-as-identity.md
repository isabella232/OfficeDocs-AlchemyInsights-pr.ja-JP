---
title: IDと同じメールアドレスを持つ複数のオブジェクト
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440545"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>IDと同じメールアドレスを持つ複数のオブジェクト

**複数のオブジェクト**

このエラーの一般的な理由の1つは、IDと同じ電子メールアドレスを持つ複数のオブジェクトが存在する場合に、Outlook Web Access の要求を適切にルーティングできないことです。 これらのオブジェクトを検索するには、次のコマンドを実行します。

· Get-Recipient <email address>

· Get-User <email address>

· Get-User <email address> -SoftDeletedUser

· Get-Contact <email address>

· Get-Mailbox <email address> -PublicFolder

· Get-Mailbox <email address> -IncludeSoftDeletedMailbox

· Get-Mailbox <email address> -InactiveMailboxOnly

この問題を解決するには、同じメール ID を持つ複数のオブジェクトを削除し、特定のメール ID を持つオブジェクトが1つあり、その受信者タイプが UserMailbox であることを確認します。

**ビジネス用および個人用のメールボックスに同じアドレスが使用されている場合**

別の原因は、ビジネス用および個人用のメールボックスに同じアドレスが使用されている場合です。 この場合、Cafe がこのシナリオをサポートするまで、ユーザーはプライマリ コンシューマー エイリアスを変更する必要があります。 これは、介入なしでは消えない永続的なエラーです。

詳細については、「[Microsoft アカウントのメールアドレスまたは電話番号を変更する](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account)」をご覧ください。