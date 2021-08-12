---
title: ワークフローが開始されない
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 77a3c022a9a3a82041b4a4a70c72c2e0940c0fba27f296f07881e3abebf1e464
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53907743"
---
# <a name="workflow-is-not-starting"></a>ワークフローが開始されない

- SharePoint 2010 および SharePoint 2013 のワークフローが開始されない。

    - ワークフローが開始されない場合は、サービスに一時的な問題が発生している可能性があります。この問題が発生すると、ワークフローの進行で断続的な遅延が発生します。 [サービスの正常性ダッシュボード](https://admin.microsoft.com/AdminPortal/Home/servicehealth)を確認して、組織が影響を受けるかどうかを調べます。

    - この問題が初めて発生してから 24 時間以上経過している場合は、サポート チケットを記録してください。多くの場合は、Microsoft が既に解決策に取り組んでいます。解決策の完成までには 24 時間以上の時間がかかります。

- SharePoint 2010 のワークフローの開始時に遅延がありました。

    - これは、ワークフローが大きなバッチでトリガーされた場合に発生します。 (たとえば、一度に複数のアイテムが追加された場合)。

    - ワークフローはリアルタイムで実行するように設計されていないため、遅延は想定通りの動作です。

   -  ワークフローが複雑な拡張可能オブジェクト マークアップ 言語 (XMOL) である場合、コンパイルに時間がかかる可能性があります。 [こちら](https://support.microsoft.com//kb/3043697)の記事を参照してください。

    - ワークフローを簡素化するか、Microsoft SharePoint 2013 ワークフローのプラットフォームの種類を使って再設計してください。

    - ワークフローの履歴が大きくなった場合は、アイテムを削除するか、新しい履歴リストを作成できます。

        詳細情報: [Purge Workflow History (ワークフロー履歴の消去)](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>関連項目
SharePoint Online で Microsoft Flow を試す方法。
- [フローを作成する](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint and Flow (SharePoint と Flow)](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
