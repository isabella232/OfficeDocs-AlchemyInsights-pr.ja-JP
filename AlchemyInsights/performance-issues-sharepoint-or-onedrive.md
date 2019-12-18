---
title: パフォーマンスの問題 - SharePoint または OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068412"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint または OneDrive において、処理が遅い、アクセスできない、または複数のユーザーで使用できない

SharePoint または OneDrive において、次のいくつかの理由で処理が遅い、アクセスできない、または、または利用できないか、サービス利用不可または 503 エラーが表示される:
  
- SharePoint または OneDrive サイトの処理が遅かったり複数のユーザーに対して遅延が生じたりする場合、一時的なサービスの問題が発生している可能性があります。そのような状況では、ユーザーが SharePoint サイトまたは OneDrive コンテンツにアクセスする際に、一時的な遅延やナビゲーション エラーが発生する可能性があります。 [サービスの正常性ダッシュボード](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)を確認して、組織が影響を受けるかどうかを調べます。
  
- ユーザーが SharePoint または OneDrive のサイトに移動しようとしたときに、「*503 サーバーがビジー状態です*」のエラーが発生することがあります。 このエラーは、SharePoint サービス内での調整が原因の可能性があります。 SharePoint Online は、SharePoint Online サービスの最適なパフォーマンスと信頼性を維持する目的で調整を使用します。 調整では、リソースの過剰な使用を防ぐため、ユーザー アクションまたは (スクリプトまたはコードによる) 同時呼び出しの数が制限されます。 調整の詳細については、「[SharePoint Online で調整またはブロックを回避する](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)」を参照してください。

- **クラシック**または**モダン**の SharePoint サイトまたはページでパフォーマンスの低下が発生した場合は、[ページ診断ツール](https://aka.ms/perftool)を利用してページの分析を行ってください。
  
- 全般的なパフォーマンス低下が引き続き発生する場合は、「[SharePoint Online のパフォーマンス チューニングの概要](https://go.microsoft.com/fwlink/?linkid=2024334)」の記事の下にあるリソースを参照してください。
  