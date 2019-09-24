---
title: 従来の SharePoint 監査ログ レポート
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068028"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>SharePoint および OneDrive 監査ログ

**SharePoint と OneDrive のモダン統合監査ログをコンプライアンス センターから実行**

- [統合監査ログを有効または無効にする](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

SharePoint または OneDrive で追加の構成は必要ありません。

- 監査ログの検索を使用して、ファイル、フォルダー、ユーザーのアクセス許可のアクティビティを確認します。

    - [ファイル アクティビティとページ アクティビティ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [フォルダー アクティビティ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [共有アクティビティとアクセス要求アクティビティ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [同期アクティビティ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [サイト管理アクティビティ](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- これらのイベントを取得する方法の詳細については、「[監査ログを検索する](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)」を参照してください。

**SharePoint クラシック監査ログ**

SPO レガシー監査を統合監査ログ (UAL) に移行しました。 これは基本的に、すべての SPO レガシー監査レポートが UAL を介して提供され、レガシー監査信号が UAL に移行されたことを意味します。

重要な変更:

- 機能としてのトリミングは使用できません。
- 監査する特定のイベントを選択するセクションは利用できません。 既定で利用可能な監査イベントの完全なリストについては、[このドキュメント](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)を参照してください。
- **カスタマイズされたレポート**の「場所」オプションは使用できません。 
- 「ドキュメントを開くまたはダウンロードする」イベントは利用できません。 

