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
ms.openlocfilehash: 83f18d06006989e03ee6095e430aaf3eb5c72c09
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714775"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>電子情報開示のエクスポート ツールをインストールまたは実行できません。

検索結果をダウンロードするために電子情報開示エクスポートツールをインストールまたは実行できない場合は、次の点を確認してください。
  
- 使用するコンピューターは、次の前提条件を満たしている必要があります:

  - 32 ビットおよび 64 ビット バージョンの Windows 7 およびそれ以降のバージョン

  - Microsoft .NET Framework 4.7

  - サポートされているブラウザー:

  - Microsoft Edge

    または

  - Internet Explorer 10 以降のバージョン

    Google Chrome や Mozilla Firefox など、他のブラウザーはサポートされていません。

- 組織が Azure のエンドポイント (**\*.blob.core.windows.net**) に接続できます (ワイルドカードはエクスポート ジョブの一意の識別子を表します)。

- Microsoft 365 セキュリティ&amp;コンプライアンスセンターで、エクスポートの役割が割り当てられていること。既定では、この役割は電子情報開示マネージャーの役割グループにのみ割り当てられます。「[電子情報開示のアクセス許可を割り当てる](https://docs.microsoft.com/office365/securitycompliance/assign-ediscovery-permissions)」をご覧ください。

詳細については、「[コンテンツ検索の結果をエクスポートする](https://docs.microsoft.com/office365/securitycompliance/export-search-results)」を参照してください。
  