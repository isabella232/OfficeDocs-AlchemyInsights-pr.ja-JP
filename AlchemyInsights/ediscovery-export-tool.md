---
title: 電子情報開示のエクスポート ツール
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: f7b7e1ae4f1f686fa510403d398c4ff750dbadb9065b8d63701a927eeac52d9b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101307"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>電子情報開示のエクスポート ツールをインストールまたは実行できません。

検索結果をダウンロードするために電子情報開示のエクスポート ツールをインストールしたり実行したりできない場合は、次のことをご確認ください。
  
- 使用するコンピューターは、次の前提条件を満たしている必要があります:

  - 32 ビットおよび 64 ビット バージョンの Windows 7 およびそれ以降のバージョン

  - Microsoft .NET Framework 4.7

  - サポートされているブラウザー:

  - Microsoft Edge

    または

  - Internet Explorer 10 以降のバージョン

    Google Chrome や Mozilla Firefox など、他のブラウザーはサポートされていません。

- 組織が Azure のエンドポイント (**\*.blob.core.windows.net**) に接続できます (ワイルドカードはエクスポート ジョブの一意の識別子を表します)。

- Microsoft 365 セキュリティ&amp;コンプライアンス センターで、ユーザーにエクスポートの役割が割り当てられています。既定では、この役割は電子情報開示管理者の役割グループにのみ割り当てられています。「[電子情報開示のアクセス許可を割り当てる](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)」を参照してください。

詳細については、「[コンテンツ検索の結果をエクスポートする](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)」を参照してください。

10 万個以上のメールボックスをエクスポートする場合は、次の Powershell を使用し、エクスポート結果をダウンロードする必要があります: 「[10 万個以上のメールボックスから結果をエクスポートする](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)」。