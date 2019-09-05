---
title: SharePoint Online の調整
ms.author: pebaum
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: d9e1400697b1e6435fea78703d2ecadc6733a57f
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751893"
---
# <a name="sharepoint-online-throttling"></a>SharePoint Online の調整

ユーザーが SharePoint または OneDrive サイトに移動しようとしたときに、503サーバーがビジー状態であるというエラーが発生することがあります。 

このエラーは、SharePoint サービス内での調整によって発生する可能性があります。 SharePoint Online は、SharePoint Online サービスの最適なパフォーマンスと信頼性を維持する目的で調整を使用します。 調整では、リソースの過剰な使用を防ぐため、ユーザー アクションまたは (スクリプトまたはコードによる) 同時呼び出しの数が制限されます。 調整された場合は、ユーザー設定コードのため、99% の時間を使用します。

調整の詳細については、「 [SharePoint Online で調整またはブロックを回避](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)する」を参照してください。

このエラーが調整に関連していないと思われる場合は、[メッセージセンター](https://portal.office.com/adminportal/home#/MessageCenter)に移動して、テナントでアクティブなメンテナンスが発生しているかどうかを確認できます。

 最後に、[[サービス正常性](https://portal.office.com/adminportal/home#/servicehealth)] ページにアクセスして、発生している可能性があるすべてのアドバイザリ/インシデントを確認してください。

