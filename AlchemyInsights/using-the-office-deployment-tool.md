---
title: Office 展開ツールを使用してください。
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: b4ade0f21794a8986aa7a37d783da5fa289488fc
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29476835"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="be5cf-102">Office 展開ツール (ODT) を使用してください。</span><span class="sxs-lookup"><span data-stu-id="be5cf-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="be5cf-p101">Office 365 のバージョンの Office を展開するのにには、Office の展開ツール (ODT) を使用します。Office 展開ツール (setup.exe) は、コマンドラインから実行され、構成 XML ファイルを使用して、Office を展開するときに適用するには、どのような設定を決定します。</span><span class="sxs-lookup"><span data-stu-id="be5cf-p101">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office. The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="be5cf-105">[Microsoft ダウンロード センター](http://go.microsoft.com/fwlink/p/?LinkID=626065)から Office の展開ツールの最新バージョンをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="be5cf-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
    
2. <span data-ttu-id="be5cf-p102">展開の設定を選択し、構成 XML ファイルを作成するには、 [Office カスタマイズ ツール (OCT)](https://config.office.com)を使用します。構成ファイルをエクスポートし、setup.exe が存在する同じフォルダーにローカルに配置します。</span><span class="sxs-lookup"><span data-stu-id="be5cf-p102">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file. Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span> 
    
    <span data-ttu-id="be5cf-p103">**注:** 問題一般的に発生する期日を正しく構成されていない Office のインストールまたは構成ファイルの不正です。このような問題を避けるためには、構成ファイルを作成するのには、Office カスタマイズ ツールを使用することをお勧めします。Office カスタマイズ ツールに既存の構成ファイルをインポートすることもできます。</span><span class="sxs-lookup"><span data-stu-id="be5cf-p103">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files. To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file. You can also import existing configuration files into the Office Customization Tool.</span></span> 
    
3. <span data-ttu-id="be5cf-p104">、管理者特権のコマンド プロンプトから setup.exe が格納されている場所にダウンロード モードでの Office の展開ツールの実行し、保存した構成ファイルを指定します。この例で、構成ファイルの名前は Configuration.xml。</span><span class="sxs-lookup"><span data-stu-id="be5cf-p104">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved. In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="be5cf-113">Office 展開ツールの実行のモードを構成し、構成ファイルを指定します。</span><span class="sxs-lookup"><span data-stu-id="be5cf-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="be5cf-114">**注:** クライアント コンピューターに Office をインストールして、そのコンピューターのローカル管理者のアクセス許可が必要この手順を実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="be5cf-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span> 
    
<span data-ttu-id="be5cf-p105">Office 展開ツールを使用して、Office 365 用リソースの展開シナリオの詳細については、 [Office の展開ツールの概要](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)を参照してください。Office カスタマイズ ツールを使用する方法の詳細については、 [Office カスタマイズ ツールの概要](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="be5cf-p105">To learn more about using Office Deployment Tool for your Office 365 ProPlus deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
  

