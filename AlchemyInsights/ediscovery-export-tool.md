---
title: 電子情報開示のエクスポート ツール
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 7e2964ef0a44ddf421e4aae007acbdbda196e20f
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769308"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>電子情報開示のエクスポート ツールをインストールまたは実行できません。

検索結果をダウンロードするために Office 365 の電子情報開示のエクスポート ツールをインストールしたり、実行することができない場合は、次のことを確認してください。
  
- 使用するコンピューターは、次の前提条件を満たしている必要があります:

  - 32 ビットおよび 64 ビット バージョンの Windows 7 およびそれ以降のバージョン

  - Microsoft .NET Framework 4.7

  - サポートされているブラウザー:

  - Microsoft Edge

    または

  - Internet Explorer 10 以降のバージョン

    Google Chrome や Mozilla Firefox など、他のブラウザーはサポートされていません。

- 組織が Azure のエンドポイント (**\*.blob.core.windows.net**) に接続できます (ワイルドカードはエクスポート ジョブの一意の識別子を表します)。

- Office 365 のセキュリティ/コンプライアンス センターで、ユーザーにエクスポートの役割が割り当てられています。既定では、この役割は電子情報開示管理者の役割グループにのみ割り当てられています。「[電子情報開示のアクセス許可を割り当てる](https://docs.microsoft.com/office365/securitycompliance/assign-ediscovery-permissions)」を参照してください。

詳細については、「[コンテンツ検索の結果をエクスポートする](https://docs.microsoft.com/office365/securitycompliance/export-search-results)」を参照してください。
  