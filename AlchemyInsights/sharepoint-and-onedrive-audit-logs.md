---
title: 従来の SharePoint 監査ログ レポート
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 0aedb549f11db54d3cd480671fb0767c60680ad3
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509605"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>SharePoint および OneDrive 監査ログ

## <a name="sharepoint-classic-audit-logs"></a>SharePoint クラシック監査ログ

SPO レガシ監査を統合監査ログ (UAL) に移行しました。 すべての SPO レガシ監査レポートが UAL を介して提供され、レガシ監査信号が UAL に移行されました。

重要な変更:

* 機能としてのトリミングは使用できません。
* 監査する特定のイベントを選択することはできません。 既定で利用可能な監査イベントの完全なリストについては、[このドキュメント](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)を参照してください。
* **カスタマイズされたレポート**の「**場所**」オプションは使用できません。
* 「**ドキュメントを開くまたはダウンロードする**」イベント オプションは利用できません。

[サイト コレクションの監査設定を構成する](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint と OneDrive のモダン統合監査ログをコンプライアンス センターから実行

* [統合監査ログを有効または無効にする](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

SharePoint または OneDrive で追加の構成は必要ありません。

監査ログの検索を使用して、ファイル、フォルダー、ユーザーのアクセス許可のアクティビティを確認します。

* [ファイル アクティビティとページ アクティビティ](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [フォルダー アクティビティ](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [共有アクティビティとアクセス要求アクティビティ](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [同期アクティビティ](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [サイト管理アクティビティ](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

これらのイベントを取得する方法の詳細については、「[監査ログを検索する](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)」を参照してください。
