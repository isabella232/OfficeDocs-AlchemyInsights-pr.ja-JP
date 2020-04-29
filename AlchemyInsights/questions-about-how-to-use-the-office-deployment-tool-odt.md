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
ms.openlocfilehash: 96d3f70f554f71c43d6458ec8debc099cd9fb040
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43698063"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="86aef-102">Office 展開ツール (ODT) の使用法に関する質問</span><span class="sxs-lookup"><span data-stu-id="86aef-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="86aef-103">[Microsoft ダウンロード センター](https://go.microsoft.com/fwlink/p/?LinkID=626065)から Office 展開ツールをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="86aef-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="86aef-104">ファイルをダウンロードした後、自己解凍実行ファイルを実行します。そこには、Office 展開ツールの実行可能ファイル (setup.exe) およびサンプル構成ファイル (configuration.xml) が含まれています。</span><span class="sxs-lookup"><span data-stu-id="86aef-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="86aef-105">**Microsoft 365 Apps for enterprise の製品をクライアント コンピューターから除外するには:**</span><span class="sxs-lookup"><span data-stu-id="86aef-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="86aef-p101">Microsoft 365 Apps for enterprise のインストール時には、特定の製品を除外することができます。これを行うには、ODT を使用した Office のインストール手順に従いますが、構成ファイルに ExcludeApp 要素を含めます。たとえば、次の構成ファイルは Publisher 以外の Microsoft 365 Apps for enterprise 製品をすべてインストールします。</span><span class="sxs-lookup"><span data-stu-id="86aef-p101">When installing Microsoft 365 Apps for enterprise, you can exclude specific products. To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file. For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="86aef-109">Office 展開ツールの概要</span><span class="sxs-lookup"><span data-stu-id="86aef-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

