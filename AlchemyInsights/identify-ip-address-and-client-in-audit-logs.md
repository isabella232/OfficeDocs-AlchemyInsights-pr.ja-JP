---
title: 監査ログで IP アドレスとクライアントを識別する
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e0119762d2a34bd2b0da827faf55c832e29d8a2b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539034"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>監査ログで IP アドレスとクライアントを識別する

Office 365 ユーザーまたは管理者によってアクティビティに対応する IP アドレスが監査ログに表示されます。 クライアント情報も記録されます。 このような情報を識別する手順は次のとおりです。

1. [Office 365 セキュリティ & コンプライアンスセンター](https://protection.office.com/)にログインします。

2. [ **** > **監査ログ**の検索] ページに移動します。

   特定のアクティビティに関心がある場合は、[**アクティビティ**] リストから選択します。 指定しない場合は、選択したユーザーに対してすべてのアクティビティが返されます (既定の設定)。

   **注**: 特定のアクティビティが [**操作**] メニューに表示されない場合があります。ただし、[**すべてのアクティビティの結果を表示する]** が選択されている場合は、これらの監査アイテムが返されます (既定の設定)。

3. [**ユーザー** ] フィールドでユーザー名を指定し、アクティビティに該当する日付の範囲を選択して、[**検索**] をクリックします。

結果には、そのアクティビティの IP アドレスが結果ウィンドウに表示されます。 監査レコードを選択して、**詳細**ポップアップ (たとえば、[クライアント]、[アクションを実行したユーザー] など) で詳細情報を表示します。

詳細については、「[危害を受けたアカウントへのアクセスに使用されたコンピューターの IP アドレスを検索する](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account)」を参照してください。
