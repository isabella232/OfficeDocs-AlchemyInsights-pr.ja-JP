---
title: Office 展開ツールの使用
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085837"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="195ad-102">Office 展開ツールの使用 (ODT)</span><span class="sxs-lookup"><span data-stu-id="195ad-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="195ad-p101">Office 展開ツール (ODT) を使用して Office の Office 365 バージョンを展開します。Office 展開ツール (setupodt.exe) はコマンド ラインから実行します。このツールでは、構成 XML ファイルを使用して、Office 展開時に適用される設定値を決定します。</span><span class="sxs-lookup"><span data-stu-id="195ad-p101">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office. The Office Deployment Tool (setupodt.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="195ad-105">[Microsoft ダウンロード センター](https://go.microsoft.com/fwlink/p/?LinkID=626065)から最新バージョンの Office 展開ツールをダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="195ad-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="195ad-p102">[Office カスタマイズ ツール (OCT)](https://config.office.com) を使用して、展開の環境設定を選択し、構成 XML ファイルを作成します。その構成ファイルをエクスポートして、setupodt.exe が置かれているのと同じフォルダーにローカルに配置します。</span><span class="sxs-lookup"><span data-stu-id="195ad-p102">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file. Export the configuration file and place it locally on the same folder where the setupodt.exe resides.</span></span>

    <span data-ttu-id="195ad-p103">**注:** Office のインストールでは、一般的に構成ファイルの構成内容または形式が正しくないことが原因で問題が発生します。このような問題を避けるために、Office カスタマイズ ツールを使用して構成ファイルを作成することをお勧めします。また、Office カスタマイズ ツールに既存の構成ファイルをインポートすることもできます。</span><span class="sxs-lookup"><span data-stu-id="195ad-p103">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files. To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file. You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="195ad-p104">管理者特権でのコマンド プロンプトから、setupodt.exe が置かれている場所に切り替えて、Office 展開ツールをダウンロード モードで実行し、先ほど保存した構成ファイルを指定します。この例では、構成ファイルに Configuration.xml という名前が付けられています。</span><span class="sxs-lookup"><span data-stu-id="195ad-p104">From an elevated command prompt, switch to the location where setupodt.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved. In this example, the configuration file is named Configuration.xml:</span></span>

```setupodt.exe /download Configuration.xml```

<span data-ttu-id="195ad-113">4. Office 展開ツールを構成モードで実行して、構成ファイルを指定します。</span><span class="sxs-lookup"><span data-stu-id="195ad-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setupodt.exe /configure Configuration.xml```

<span data-ttu-id="195ad-114">**注:** この手順は、Office をインストールするクライアント コンピューターから実行する必要があります。また、そのコンピューターに対してローカル管理者のアクセス許可を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="195ad-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="195ad-p105">Microsoft 365 Apps for enterprise の展開シナリオに Office 展開ツールを使用する方法の詳細については、「[Office 展開ツールの概要](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)」を参照してください。Office カスタマイズ ツールの使用方法の詳細については、「[Office カスタマイズ ツールの概要](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="195ad-p105">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
