---
title: IDと同じメールアドレスを持つ複数のオブジェクト
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: 5866d182cb2e97e37bc6df87e05fb6ef55bfed1d36f9daa95b7b8993a509e2dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011917"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>IDと同じメールアドレスを持つ複数のオブジェクト

**複数のオブジェクト**

このエラーの一般的な理由の 1 つは、ID と同じメール アドレスを持つ複数のオブジェクトが存在する場合に、Outlook Web アクセス要求を正しくルーティングできないことです。これらのオブジェクトを検索するには、次のコマンドを実行します。

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