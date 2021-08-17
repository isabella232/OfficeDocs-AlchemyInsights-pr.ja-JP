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
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083775"
---
# <a name="using-the-office-deployment-tool-odt"></a>Office 展開ツールの使用 (ODT)

Office 展開ツール (ODT) を使用して Office の Office 365 バージョンを展開します。Office 展開ツール (setup.exe) はコマンド ラインから実行します。このツールでは、構成 XML ファイルを使用して、Office 展開時に適用される設定値を決定します。
  
1. [Microsoft ダウンロード センター](https://go.microsoft.com/fwlink/p/?LinkID=626065)から最新バージョンの Office 展開ツールをダウンロードします。

2. [Office カスタマイズ ツール (OCT)](https://config.office.com) を使用して、展開の環境設定を選択し、構成 XML ファイルを作成します。その構成ファイルをエクスポートして、setup.exe が置かれているのと同じフォルダーにローカルに配置します。

    **注:** Office のインストールでは、一般的に構成ファイルの構成内容または形式が正しくないことが原因で問題が発生します。このような問題を避けるために、Office カスタマイズ ツールを使用して構成ファイルを作成することをお勧めします。また、Office カスタマイズ ツールに既存の構成ファイルをインポートすることもできます。

3. 管理者特権でのコマンド プロンプトから、setup.exe が置かれている場所に切り替えて、Office 展開ツールをダウンロード モードで実行し、先ほど保存した構成ファイルを指定します。この例では、構成ファイルに Configuration.xml という名前が付けられています。

```setup.exe /download Configuration.xml```

4. Office 展開ツールを構成モードで実行して、構成ファイルを指定します。

```setup.exe /configure Configuration.xml```

**注:** この手順は、Office をインストールするクライアント コンピューターから実行する必要があります。また、そのコンピューターに対してローカル管理者のアクセス許可を持っている必要があります。

Microsoft 365 Apps for enterprise の展開シナリオに Office 展開ツールを使用する方法の詳細については、「[Office 展開ツールの概要](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)」を参照してください。Office カスタマイズ ツールの使用方法の詳細については、「[Office カスタマイズ ツールの概要](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)」を参照してください。
