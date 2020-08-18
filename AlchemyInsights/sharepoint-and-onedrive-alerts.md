---
title: SharePoint および OneDrive のアラートの受信の遅延
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 92e517ae6e83aa91b9838047ec77759dc893bc57
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/17/2020
ms.locfileid: "46785670"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>SharePoint および OneDrive のアラートの受信の遅延

- まずは、メールの迷惑メール フォルダーまたはスパム フォルダーを確認します。
- **複数のファイルまたはライブラリからのすべてのアラートの配信に遅延がある**場合は、[サービス正常性ダッシュボード](https://portal.office.com/adminportal/home?ref=/servicehealth)にアクセスして SharePoint または Exchange で発生している可能性のあるアドバイザリやインシデントを確認します。 問題は、SharePoint のアラート機能または Exchange を介したメールの遅延にある可能性があります。 また、他のメールが配信されているかどうかにも注意してください。もしも配信されていない場合には、おそらく問題は Exchange の遅延にあります。
- **特定のファイルまたはライブラリからの個別のアラートが配信されない**場合には、削除して再作成してみてください。 詳細については、「[SharePoint アラートの管理、表示、または削除](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2)」を参照してください。

> [!NOTE]
> - アラートを配布グループに送信することはできません。 セキュリティおよび O365 グループのみがサポートされています。
> - アラートのメール テンプレートをカスタマイズすることはできません。 これらを実現するには、Microsoft Flow または SharePoint Designer ワークフローを使用する必要があります。
