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
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28298167"
---
<span data-ttu-id="dad2a-p101">のみ、ユーザーが Exchange のライセンスを持っている場合、ユーザーのメールボックスを共有されているメールボックスを変換できます。メールボックスを変換すると、引き続きそのリストには、共有メールボックスが含まれているため、アクティブなユーザーの一覧に表示します。ただし、変換後のメールボックスも表示されます、共有されているメールボックスの一覧で。</span><span class="sxs-lookup"><span data-stu-id="dad2a-p101">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license. After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes. However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="dad2a-p102">Exchange 管理コンソールでメールボックスを変換しようとする場合は、変換が失敗した場合は、ブラウザーのキャッシュと cookie をオフにしてからやり直してください。それでも機能しない場合は、次のコマンドを実行して、Exchange 管理シェルでメールボックスを変換するを実行してください。</span><span class="sxs-lookup"><span data-stu-id="dad2a-p102">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again. If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="dad2a-107">メールボックス変換の詳細は、[ユーザーのメールボックス、共有メールボックスへの変換](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba)で使用されています。</span><span class="sxs-lookup"><span data-stu-id="dad2a-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
