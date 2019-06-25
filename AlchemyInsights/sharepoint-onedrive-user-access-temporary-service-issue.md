---
title: パフォーマンスの問題 - SharePoint または OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 745a62c917c0b94501843332d70609261c6d3b76
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "35174471"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint または OneDrive において、処理が遅い、アクセスできない、または複数のユーザーで使用できない

以前にアクセスしたことがある複数のユーザーが OneDrive または SharePoint サイトを使用できない場合は、一時的なサービスの問題が発生する可能性があります。 [サービス正常性ダッシュボードをチェックし](https://portal.office.com/adminportal/home#/servicehealth)ます。

ユーザーを追加してライセンスを付与する

[Office 365 for business のユーザーにライセンスを割り当てる](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)ようにしてください。


**アクセス許可の割り当て**

ユーザーに Sharepoint ライセンスが割り当てられていて、アクセス拒否メッセージが依然として受信されている場合は、それらのユーザーに[適切なアクセス許可レベル](https://docs.microsoft.com/sharepoint/understanding-permission-levels)が割り当てられていることを確認してください。

**アクセス要求機能の使用を検討する**

[アクセス要求機能](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3)を使用すると、ユーザーが現在表示する権限を持っていないコンテンツへのアクセス権を要求できます。

**カスタムスクリプトを許可すると、アクセス拒否の問題が発生することがある**

特定のシナリオでは、[*カスタムスクリプトを許可*する] 機能がアクセス拒否を提示している可能性があります。 影響を受ける機能の一覧については、セキュリティに関する考慮事項と、この機能を無効にする機能を示します。 [[ユーザー設定スクリプトの許可または禁止](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)] を参照してください。

