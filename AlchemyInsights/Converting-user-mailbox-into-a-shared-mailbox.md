---
title: 共有されているメールボックス ユーザーのメールボックスに変換しますか。
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Priority
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 22ad1b3fb818b40bcd77974031735f931e986968
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29476826"
---
のみ、ユーザーが Exchange のライセンスを持っている場合、ユーザーのメールボックスを共有されているメールボックスを変換できます。メールボックスを変換すると、引き続きそのリストには、共有メールボックスが含まれているため、アクティブなユーザーの一覧に表示します。ただし、変換後のメールボックスも表示されます、共有されているメールボックスの一覧で。 
  
Exchange 管理コンソールでメールボックスを変換しようとする場合は、変換が失敗した場合は、ブラウザーのキャッシュと cookie をオフにしてからやり直してください。それでも機能しない場合は、次のコマンドを実行して、Exchange 管理シェルでメールボックスを変換するを実行してください。
  
```
Set-Mailbox -Type Shared
```

メールボックス変換の詳細は、[ユーザーのメールボックス、共有メールボックスへの変換](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba)で使用されています。
  
