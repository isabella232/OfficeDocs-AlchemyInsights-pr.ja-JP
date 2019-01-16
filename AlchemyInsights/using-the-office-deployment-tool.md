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
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28297955"
---
# <a name="using-the-office-deployment-tool-odt"></a>Office 展開ツール (ODT) を使用してください。

Office 365 のバージョンの Office を展開するのにには、Office の展開ツール (ODT) を使用します。Office 展開ツール (setup.exe) は、コマンドラインから実行され、構成 XML ファイルを使用して、Office を展開するときに適用するには、どのような設定を決定します。
  
1. [Microsoft ダウンロード センター](http://go.microsoft.com/fwlink/p/?LinkID=626065)から Office の展開ツールの最新バージョンをダウンロードします。
    
2. 展開の設定を選択し、構成 XML ファイルを作成するには、 [Office カスタマイズ ツール (OCT)](https://config.office.com)を使用します。構成ファイルをエクスポートし、setup.exe が存在する同じフォルダーにローカルに配置します。 
    
    **注:** 問題一般的に発生する期日を正しく構成されていない Office のインストールまたは構成ファイルの不正です。このような問題を避けるためには、構成ファイルを作成するのには、Office カスタマイズ ツールを使用することをお勧めします。Office カスタマイズ ツールに既存の構成ファイルをインポートすることもできます。 
    
3. 、管理者特権のコマンド プロンプトから setup.exe が格納されている場所にダウンロード モードでの Office の展開ツールの実行し、保存した構成ファイルを指定します。この例で、構成ファイルの名前は Configuration.xml。
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Office 展開ツールの実行のモードを構成し、構成ファイルを指定します。
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **注:** クライアント コンピューターに Office をインストールして、そのコンピューターのローカル管理者のアクセス許可が必要この手順を実行する必要があります。 
    
Office 展開ツールを使用して、Office 365 用リソースの展開シナリオの詳細については、 [Office の展開ツールの概要](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)を参照してください。Office カスタマイズ ツールを使用する方法の詳細については、 [Office カスタマイズ ツールの概要](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)を参照してください。
  

