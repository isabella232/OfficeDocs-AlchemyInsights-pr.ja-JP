---
title: SharePoint および OneDrive 通知を受信しない
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
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/26/2019
ms.locfileid: "37313934"
---
# <a name="not-receiving-sharepoint-and-onedrive-alerts"></a>SharePoint および OneDrive 通知を受信しない

まず、電子メールの [迷惑メール] フォルダーまたは [スパム] フォルダーをチェックします。

次に、**すべての通知が配信されてい**ないか、特定のファイルまたはライブラリからの**個々の通知**が配信されていないかを確認します。

- **複数のファイルまたはライブラリからのすべての通知が配信**されない場合は、[サービス正常性ダッシュボード](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fadmin.microsoft.com%2FAdminPortal%2FHome%23%2Fservicehealth&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0)にアクセスして、SharePoint または Exchange で発生している可能性があるすべてのアドバイザリ/インシデントをチェックします。 この問題は、Exchange による電子メールの SharePoint 通知機能または遅延が原因である可能性があります。 また、他のメールが配信されているかどうかにも注意してください。そうでない場合は、Exchange の遅延が原因である可能性があります。
- **特定のファイルまたはライブラリからの個々の通知が配信されない**場合は、削除して再作成します。 通知を再作成するには、「 [SharePoint alerts を管理、表示、または削除](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2Fmanage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2%3Fui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax%2Fepn3E%3D&reserved=0)する」を参照してください。

> [!NOTE]
> - 通知を配布グループに送信することはできません。 セキュリティと O365 グループのみがサポートされています。
> - 通知電子メールテンプレートをカスタマイズすることはできません。 これらを実現するには、Microsoft Flow または SharePoint Designer ワークフローを使用する必要があります。
