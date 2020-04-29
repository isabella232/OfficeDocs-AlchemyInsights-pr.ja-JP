---
title: '[エクスプローラーで開く] が機能しない'
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713039"
---
# <a name="open-with-explorer-isnt-working"></a>[エクスプローラーで開く] が機能していない

[**エクスプローラーで開く**] または [**エクスプローラーで表示**] が機能しない場合は、以下の手順に従って WebClient サービスが [**実行中**] に設定されていることを確認します。このサービスが実行されていない場合、たとえば、SharePoint または OneDrive のライブラリを開くのに長時間かかることがあります。 
  
1. Windows の検索ボックスに "実行" と入力し、[ファイル名を指定して実行] を選択した後、"services.msc" と入力して **Enter**キーを押します。
    
2. WebClient サービスまでスクロール ダウンし、[**状態**] 列を確認します。WebClient サービスの状態が [**実行中**] ではない場合、サービスをダブルクリックして、[**開始**]、[**OK**] の順にクリックします。必要に応じて、[**スタートアップの種類**] ボックスで [**手動**] または [**自動**] を選択して、サービスを有効にします。 
    
> [!NOTE]
> エクスプローラーで開けない問題をトラブルシューティングするには、「[エクスプローラーで開く](https://go.microsoft.com/fwlink/?linkid=871665)」を参照してください。同期の有効な代替手段については、「[OneDrive の次世代同期クライアントを使用して SharePoint ファイルを同期する](https://go.microsoft.com/fwlink/?linkid=871666)」を参照してください。 
  

