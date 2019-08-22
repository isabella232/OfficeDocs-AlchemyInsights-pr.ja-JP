---
title: SharePoint Online の調整
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: c7881c0c7331e0aa74fcc439f52157bb75a56160
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559846"
---
# <a name="sharepoint-online-throttling"></a>SharePoint Online の調整

ユーザーが SharePoint または OneDrive のサイトに移動しようとしたときに、"503 サーバーがビジー状態です" のエラーが発生することがあります。 

このエラーは、SharePoint サービス内での調整が原因の可能性があります。 SharePoint Online は、SharePoint Online サービスの最適なパフォーマンスと信頼性を維持する目的で調整を使用します。 調整では、リソースの過剰な使用を防ぐため、ユーザー アクションまたは (スクリプトまたはコードによる) 同時呼び出しの数が制限されます。 調整の対象になる場合、99% の確率でカスタム コードが原因であるといえます。

調整の詳細については、「[SharePoint Online で調整またはブロックを回避する](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)」を参照してください。

このエラーが調整に関連していないと考えられる場合は、[メッセージ センター](https://portal.office.com/adminportal/home#/MessageCenter)に移動して、テナントでアクティブ メンテナンスが実施されているかどうかを確認します。

 最後に、[サービス正常性](https://portal.office.com/adminportal/home#/servicehealth)ページにアクセスして、発生している可能性のあるインシデント/アドバイザリを確認してください。

