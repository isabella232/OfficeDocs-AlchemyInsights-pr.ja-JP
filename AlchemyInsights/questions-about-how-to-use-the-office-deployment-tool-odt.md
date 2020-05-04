---
title: Office 展開ツール (ODT) の使用法に関する質問
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 4aef42df4dde17d15863fca67e41f0ff23e506dc
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010754"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Office 展開ツール (ODT) の使用法に関する質問

[Microsoft ダウンロード センター](https://go.microsoft.com/fwlink/p/?LinkID=626065)から Office 展開ツールをダウンロードします。
  
ファイルをダウンロードした後、自己解凍実行ファイルを実行します。そこには、Office 展開ツールの実行可能ファイル (setup.exe) およびサンプル構成ファイル (configuration.xml) が含まれています。
  
 **Microsoft 365 Apps for enterprise の製品をクライアント コンピューターから除外するには:**
  
Microsoft 365 Apps for enterprise のインストール時には、特定の製品を除外することができます。これを行うには、ODT を使用した Office のインストール手順に従いますが、構成ファイルに ExcludeApp 要素を含めます。たとえば、次の構成ファイルは Publisher 以外の Microsoft 365 Apps for enterprise 製品をすべてインストールします。
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Office 展開ツールの概要](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

