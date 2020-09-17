---
title: SharePoint Online の調整
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 21d0f8d0118d92562b425921742513157563b5fb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773852"
---
# <a name="sharepoint-online-throttling"></a>SharePoint Online の調整

**重要**: これらの前例のない時期にも、SharePoint Online および OneDrive サービスの可用性を維持するための措置を講じています。詳細については、「[SharePoint Online の一時的な機能調整](https://aka.ms/ODSPAdjustments)」を参照してください。

**「503 サーバーがビジー状態です」のエラー**

ユーザーが SharePoint または OneDrive のサイトに移動しようとしたときに、"503 サーバーがビジー状態です" のエラーが発生することがあります。 

このエラーは、SharePoint サービス内での調整が原因の可能性があります。 SharePoint Online は、SharePoint Online サービスの最適なパフォーマンスと信頼性を維持する目的で調整を使用します。 調整では、リソースの過剰な使用を防ぐため、ユーザー アクションまたは (スクリプトまたはコードによる) 同時呼び出しの数が制限されます。 

調整の詳細については、「[SharePoint Online で調整またはブロックを回避する](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)」を参照してください。

このエラーが調整に関連していないと考えられる場合は、[メッセージ センター](https://portal.office.com/adminportal/home#/MessageCenter)に移動して、テナントでアクティブ メンテナンスが実施されているかどうかを確認します。

 最後に、[サービス正常性](https://portal.office.com/adminportal/home#/servicehealth)ページにアクセスして、発生している可能性のあるインシデント/アドバイザリを確認してください。

