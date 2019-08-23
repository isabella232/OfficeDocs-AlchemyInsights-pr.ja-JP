---
title: ワークフローが開始されていません
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: d4bfdb44c04eb6838f4a265e55a4873d14c78f6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36557981"
---
# <a name="workflow-is-not-starting"></a>ワークフローが開始されていません

- SharePoint 2010 と SharePoint 2013 ワークフローが開始していません。

    - ワークフローが開始されていない場合、ワークフローの進行状況で断続的に遅延が発生する可能性がある一時的なサービスの問題が発生する可能性があります。 [サービス正常性ダッシュボード](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth)をチェックして、組織が影響を受けているかどうかを確認します。

    - この問題が最初に発生してから24時間以上経過している場合は、サポートチケットをログに記録してください。 多くの場合、すでに解決策に取り組んでいます。 解決策を完成させるために少なくとも 24 時間を与えてください。

- SharePoint 2010 のワークフローが開始時に遅延します。

    - これは、ワークフローが大きなバッチでトリガーされた場合に発生します。 (たとえば、一度に複数のアイテムが追加された場合)。

    - ワークフローはリアルタイムで実行するように設計されていないため、遅延はデザインの動作になります。

   -  ワークフローが複雑な拡張可能なオブジェクトマークアップ言語 (XMOL) の場合、コンパイルが遅くなることがあります。 [この](https://support.microsoft.com/en-us/kb/3043697)記事を確認してください。

    - ワークフローを簡素化するか、Microsoft SharePoint 2013 ワークフロープラットフォームの種類を使用して再設計する必要があります。

    - ワークフロー履歴が大きくなっている場合は、アイテムを削除するか、新しい履歴リストを作成することができます。

        詳細情報:[ワークフロー履歴の削除](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>関連項目
SharePoint Online で Microsoft Flow を試す場合
- [フローを作成する](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint およびフロー](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


