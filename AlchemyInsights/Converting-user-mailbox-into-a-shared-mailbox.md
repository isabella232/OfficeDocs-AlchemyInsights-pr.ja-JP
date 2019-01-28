---
title: ユーザー メールボックスを共有メールボックスに変換する場合
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
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29476826"
---
ユーザーが Exchange のライセンスを持っている場合にのみ、ユーザー メールボックスを共有メールボックスに変換できます。メールボックスを変換すると、それは引き続きアクティブなユーザーの一覧に表示されます。これは、その一覧に共有メールボックスが含まれているからです。ただし、変換されたメールボックスは共有メールボックスの一覧にも表示されます。 
  
Exchange 管理コンソールでメールボックスを変換しようとして、変換が失敗した場合は、ブラウザーのキャッシュと Cookie をクリアしてからやり直してください。それでも動作しない場合は、次のコマンドを実行して、Exchange 管理シェルでメールボックスを変換してみてください。
  
```
Set-Mailbox -Type Shared
```

メールボックスの変換の詳細については、「[ユーザー メールボックスを共有メールボックスに変換する](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba)」を参照してください。
  
