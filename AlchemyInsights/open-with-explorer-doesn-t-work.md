---
title: エクスプ ローラーで開くが機能しません。
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: b55fc7bd5670e655334ef7be368b245c8899633a
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28297112"
---
# <a name="open-with-explorer-isnt-working"></a>エクスプ ローラーで開くが機能しません。

**エクスプ ローラーで開く**か、**ファイル エクスプ ローラー ビュー**が機能しない場合は、WebClient サービスは、以下の手順で**実行中**に設定されていることを確認します。たとえば、サービスが実行されていない場合、SharePoint または OneDrive のライブラリを開くまでに時間がかかる場合があります。 
  
1. Windows 検索ボックスで、これを実行すると、型には、実行デスクトップ アプリケーション、タイプ services.msc」と選択し、 **Enter**を選択します。
    
2. WebClient サービスまでスクロールし、[**状態**] 列を確認します。WebClient サービスの状態でない場合**を実行している**サービスをダブルクリックして**開始**] をクリック、[ **OK**] をクリックします。**[スタートアップの種類**] ボックスに**手動**または**自動**のいずれかを選択することによって、必要な場合は、サービスを有効にします。 
    
> [!NOTE]
> ファイル エクスプ ローラーで開くときの問題のトラブルシューティングを行うには、[エクスプ ローラーで開く](https://go.microsoft.com/fwlink/?linkid=871665)を参照してください。良い代替案としての同期を表示:[新しい OneDrive 同期クライアントと同期 SharePoint ファイル](https://go.microsoft.com/fwlink/?linkid=871666)です。 
  

