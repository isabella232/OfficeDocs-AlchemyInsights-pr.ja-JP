---
title: 126 OWA で「メールボックスが見つかりませんでした」というエラーが表示される場合
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 4/9/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: b7d54e9fb29bf94ec540e6059e932ec33f326495
ms.sourcegitcommit: c003a5db7edc3a44fb5b31b46cd45f12b62d172a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/22/2019
ms.locfileid: "30209814"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Outlook on the web で「メールボックスが見つかりませんでした」というエラーが表示される場合

Outlook on the web を使用しているときに、「**メールボックスが見つかりませんでした**」というエラーが表示された場合は、Outlook on the web への接続時に使用したアカウントに Exchange Online ライセンスが付与されていないため、そのアカウントにメールボックスが関連付けられていません。管理者は、次の手順に従ってアカウントにライセンスを割り当てることができます。 
  
1. [Microsoft 365 管理センター](https://portal.office.com/adminportal/home#/homepage)を開いて、**[アクティブなユーザー]** で、**[ユーザーの編集]** を選択します。
    
2. 開いた **[ユーザーの編集]** ページで、ユーザーを選択します。開いた [ユーザーのプロパティ] ページで、**[製品のライセンス]** の **[編集]** をクリックします。
    
3. 開いた **[製品のライセンス]** ページで、該当する **[場所]** の値を選択し、Exchange Online を含むライセンスを割り当てます (ライセンスを展開して、その詳細を表示します)。完了したら、**[保存]** をクリックします。
    

