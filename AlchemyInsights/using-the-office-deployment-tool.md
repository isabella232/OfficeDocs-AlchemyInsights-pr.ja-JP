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
# <a name="using-the-office-deployment-tool-odt"></a>Office 展開ツールの使用 (ODT)

Office 展開ツール (ODT) を使用して Office の Office 365 バージョンを展開します。Office 展開ツール (setup.exe) はコマンド ラインから実行します。このツールでは、構成 XML ファイルを使用して、Office 展開時に適用される設定値を決定します。
  
1. [Microsoft ダウンロード センター](https://go.microsoft.com/fwlink/p/?LinkID=626065)から最新バージョンの Office 展開ツールをダウンロードします。

2. [Office カスタマイズ ツール (OCT)](https://config.office.com) を使用して、展開の環境設定を選択し、構成 XML ファイルを作成します。その構成ファイルをエクスポートして、setup.exe が置かれているのと同じフォルダーにローカルに配置します。

    **注:** Office のインストールでは、一般的に構成ファイルの構成内容または形式が正しくないことが原因で問題が発生します。このような問題を避けるために、Office カスタマイズ ツールを使用して構成ファイルを作成することをお勧めします。また、Office カスタマイズ ツールに既存の構成ファイルをインポートすることもできます。

3. 管理者特権でのコマンド プロンプトから、setup.exe が置かれている場所に切り替えて、Office 展開ツールをダウンロード モードで実行し、先ほど保存した構成ファイルを指定します。この例では、構成ファイルに Configuration.xml という名前が付けられています。
    
  ```
  setup.exe /download Configuration.xml  
  ```

4. Office 展開ツールを構成モードで実行して、構成ファイルを指定します。
    
  ```
  setup.exe /configure Configuration.xml
  ```

    **注:** この手順は、Office をインストールするクライアント コンピューターから実行する必要があります。また、そのコンピューターに対してローカル管理者のアクセス許可を持っている必要があります。

Office 展開ツールを使用してエンタープライズ展開シナリオの Microsoft 365 アプリを使用する方法の詳細については、「 [Office 展開ツールの概要](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)」を参照してください。Office カスタマイズツールの使用方法の詳細については、「 [Office カスタマイズツールの概要](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)」を参照してください。
