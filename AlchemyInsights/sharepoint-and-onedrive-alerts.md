---
title: SharePoint および OneDrive のアラートを受信しない
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/25/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 80423791ad558fc414d50608c73f823036432e14
ms.sourcegitcommit: 5e6a805fb0b41d714ca1cf90e23b8e2daa90f90e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/26/2019
ms.locfileid: "37313934"
---
# <a name="not-receiving-sharepoint-and-onedrive-alerts"></a>SharePoint および OneDrive のアラートを受信しない

まずは、メールの迷惑メール フォルダーまたはスパム フォルダーを確認します。

次に、**すべてのアラートが配信されていない**のか、それとも特定のファイルまたはライブラリからの**個別のアラート**が配信されていないのかを判断します。

- **複数のファイルまたはライブラリからのすべてのアラートが配信されていない**場合は、[サービス正常性ダッシュボード](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fadmin.microsoft.com%2FAdminPortal%2FHome%23%2Fservicehealth&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0)にアクセスして SharePoint または Exchange で発生している可能性のあるアドバイザリやインシデントを確認します。 問題は、SharePoint のアラート機能または Exchange を介したメールの遅延にある可能性があります。 また、他のメールが配信されているかどうかにも注意してください。もしも配信されていない場合には、おそらく問題は Exchange の遅延にあります。
- **特定のファイルまたはライブラリからの個別のアラートが配信されない**場合には、削除して再作成してみてください。 詳細については、「[SharePoint アラートの管理、表示、または削除](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2Fmanage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2%3Fui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax%2Fepn3E%3D&reserved=0)」を参照してください。

> [!NOTE]
> - アラートを配布グループに送信することはできません。 セキュリティおよび O365 グループのみがサポートされています。
> - アラートのメール テンプレートをカスタマイズすることはできません。 これらを実現するには、Microsoft Flow または SharePoint Designer ワークフローを使用する必要があります。
