---
title: SharePoint および OneDrive のアラートの受信の遅延
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 02/04/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 0bc9f614047e06e8654a9b3ff64e87427f33139f
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/04/2020
ms.locfileid: "41771220"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>SharePoint および OneDrive のアラートの受信の遅延

- まずは、メールの迷惑メール フォルダーまたはスパム フォルダーを確認します。
- **複数のファイルまたはライブラリからのすべてのアラートの配信に遅延がある**場合は、[サービス正常性ダッシュボード](https://nam06.safelinks.protection.outlook.com/?url=https://admin.microsoft.com/AdminPortal/Home%23/servicehealth&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0)にアクセスして SharePoint または Exchange で発生している可能性のあるアドバイザリやインシデントを確認します。 問題は、SharePoint のアラート機能または Exchange を介したメールの遅延にある可能性があります。 また、他のメールが配信されているかどうかにも注意してください。もしも配信されていない場合には、おそらく問題は Exchange の遅延にあります。
- **特定のファイルまたはライブラリからの個別のアラートが配信されない**場合には、削除して再作成してみてください。 詳細については、「[SharePoint アラートの管理、表示、または削除](https://nam06.safelinks.protection.outlook.com/?url=https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7c01%7cv-todmc%40microsoft.com%7c2cd2037aa7304711d2bc08d741fae254%7c72f988bf86f141af91ab2d7cd011db47%7c1%7c0%7c637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax/epn3E%3D&reserved=0)」を参照してください。

> [!NOTE]
> - アラートを配布グループに送信することはできません。 セキュリティおよび O365 グループのみがサポートされています。
> - アラートのメール テンプレートをカスタマイズすることはできません。 これらを実現するには、Microsoft Flow または SharePoint Designer ワークフローを使用する必要があります。
