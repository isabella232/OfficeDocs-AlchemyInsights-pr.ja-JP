---
title: 毎日のメールの制限を超えました。 ワークフローは中断されます。
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 802aba696da61be5f0a6c12072842cbc3cd96499
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/02/2019
ms.locfileid: "36180405"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>毎日のメールの制限を超えました。 ワークフローは中断されます。

このエラーは、次のシナリオで受け取ることがあります。

- SharePoint Online に、SharePoint 2010 または SharePoint 2013 ワークフロー プラットフォームの種類を使用しているワークフローがあります。
- ワークフローは、ユーザー設定のメール メッセージを一度に 200 を超えるユーザー、または 1 日に 1 万を超える受信者に送信するか、1 分あたり 30 件を超えるメッセージを送信するように、構成されています。
- ワークフローを実行すると、電子メールメッセージは送信されず、次のような現象が発生します。
    - SharePoint 2013 プラットフォームの種類を使用するワークフローの場合は、[**ワークフローの状態**] ページを参照します。 [ワークフローの状態] ページで、[**内部の状態**] が [**開始**] に設定されており、情報のバルーンが**受信者に送信できない**ように表示されます。

この問題を回避するには、 [Exchange Online の送信者の制限](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)を超えずに電子メールメッセージを送信するようにワークフローを構成します。 たとえば、ワークフローで一時停止を使用するか、Office 365 グループ、配布グループまたはメールが有効なセキュリティグループに電子メールを送信するか、またはメッセージを1度に200人より少ない受信者に送信します。


詳細については、次の[記事](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)を参照してください。

## <a name="related-topics"></a>関連項目
- [フローを作成する](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint およびフロー](https://flow.microsoft.com/blog/sharepoint-and-flow/) 