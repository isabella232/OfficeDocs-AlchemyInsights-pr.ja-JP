---
title: ユーザー メールボックスを共有メールボックスに変換する場合
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 4da54121763fd33aa111f3bb3c26963cd271dc51
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906737"
---
<span data-ttu-id="7dd95-p101">ユーザーが Exchange のライセンスを持っている場合にのみ、ユーザー メールボックスを共有メールボックスに変換できます。メールボックスを変換すると、それは引き続きアクティブなユーザーの一覧に表示されます。これは、その一覧に共有メールボックスが含まれているからです。ただし、変換されたメールボックスは共有メールボックスの一覧にも表示されます。</span><span class="sxs-lookup"><span data-stu-id="7dd95-p101">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license. After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes. However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="7dd95-p102">Exchange 管理コンソールでメールボックスを変換しようとして、変換が失敗した場合は、ブラウザーのキャッシュと Cookie をクリアしてからやり直してください。それでも動作しない場合は、次のコマンドを実行して、Exchange 管理シェルでメールボックスを変換してみてください。</span><span class="sxs-lookup"><span data-stu-id="7dd95-p102">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again. If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="7dd95-107">メールボックスの変換の詳細については、「[ユーザー メールボックスを共有メールボックスに変換する](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7dd95-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
