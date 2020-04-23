---
title: Office 展開ツールの使用
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: fa40fef0de9b2e0e1fc329269c24e8bca9ed4146
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726253"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="bbcf6-102">Office 展開ツールの使用 (ODT)</span><span class="sxs-lookup"><span data-stu-id="bbcf6-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="bbcf6-p101">Office 展開ツール (ODT) を使用して Office の Office 365 バージョンを展開します。Office 展開ツール (setup.exe) はコマンド ラインから実行します。このツールでは、構成 XML ファイルを使用して、Office 展開時に適用される設定値を決定します。</span><span class="sxs-lookup"><span data-stu-id="bbcf6-p101">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office. The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="bbcf6-105">[Microsoft ダウンロード センター](https://go.microsoft.com/fwlink/p/?LinkID=626065)から最新バージョンの Office 展開ツールをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="bbcf6-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="bbcf6-p102">[Office カスタマイズ ツール (OCT)](https://config.office.com) を使用して、展開の環境設定を選択し、構成 XML ファイルを作成します。その構成ファイルをエクスポートして、setup.exe が置かれているのと同じフォルダーにローカルに配置します。</span><span class="sxs-lookup"><span data-stu-id="bbcf6-p102">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file. Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="bbcf6-p103">**注:** Office のインストールでは、一般的に構成ファイルの構成内容または形式が正しくないことが原因で問題が発生します。このような問題を避けるために、Office カスタマイズ ツールを使用して構成ファイルを作成することをお勧めします。また、Office カスタマイズ ツールに既存の構成ファイルをインポートすることもできます。</span><span class="sxs-lookup"><span data-stu-id="bbcf6-p103">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files. To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file. You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="bbcf6-p104">管理者特権でのコマンド プロンプトから、setup.exe が置かれている場所に切り替えて、Office 展開ツールをダウンロード モードで実行し、先ほど保存した構成ファイルを指定します。この例では、構成ファイルに Configuration.xml という名前が付けられています。</span><span class="sxs-lookup"><span data-stu-id="bbcf6-p104">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved. In this example, the configuration file is named Configuration.xml:</span></span>
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. <span data-ttu-id="bbcf6-113">Office 展開ツールを構成モードで実行して、構成ファイルを指定します。</span><span class="sxs-lookup"><span data-stu-id="bbcf6-113">Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>
    
  ```
  setup.exe /configure Configuration.xml
  ```

    <span data-ttu-id="bbcf6-114">**注:** この手順は、Office をインストールするクライアント コンピューターから実行する必要があります。また、そのコンピューターに対してローカル管理者のアクセス許可を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bbcf6-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="bbcf6-p105">Office 展開ツールを使用してエンタープライズ展開シナリオの Microsoft 365 アプリを使用する方法の詳細については、「 [Office 展開ツールの概要](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)」を参照してください。Office カスタマイズツールの使用方法の詳細については、「 [Office カスタマイズツールの概要](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bbcf6-p105">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool). For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
