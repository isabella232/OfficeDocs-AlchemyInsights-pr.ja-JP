---
title: 電子情報開示のエクスポート用に Chromium ブラウザー ベースの Microsoft Edge を使用する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3473"
- "3100022"
ms.openlocfilehash: d4ccaf4928fb041ec7914b95520c4e7ccdac208c
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2019
ms.locfileid: "40791278"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a>電子情報開示のエクスポート用に Chromium ブラウザー ベースの Microsoft Edge を使用する

最近行われた変更により、Microsoft Edge ブラウザーでは、ClickOnce のサポートが既定では有効化されないようになりました。 Microsoft Office 365 電子情報開示エクスポート ツールを継続して使用するには、Microsoft Internet Explorer を使用するか、Microsoft Edge での ClickOnce のサポートを有効にする必要があります。 

Chromium に基づく Microsoft Edge で ClickOnce のサポートを有効にするには、次の操作を行います。 
1. Microsoft Edge ブラウザーで、edge://flags/#edge-click-once にアクセスします。
2. [ClickOnce Support] オプションで、値を [**Default (規定)**] または [**Disabled (無効)**] から [**Enabled (有効)**] に変更します。 
3. ブラウザー ウィンドウの下部で、[**Restart (リスタート)**] を選択します。 <br>
 Microsoft Edge を再起動すると、変更が有効になります。 

この手順およびエクスポート ツールをインストールする手順の詳細については、「[コンテンツ検索の結果をエクスポートする](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)」を参照してください。