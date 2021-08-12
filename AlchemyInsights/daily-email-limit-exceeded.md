---
title: 1 日のメールの制限を超えました。 ワークフローは中断されています。
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914656"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>1 日のメールの制限を超えました。ワークフローは中断されています。

このエラーは、次のシナリオに該当する場合に受信する可能性があります。

- SharePoint Online に、SharePoint 2010 または SharePoint 2013 ワークフロー プラットフォームの種類を使用しているワークフローがあります。
- ワークフローは、ユーザー設定のメール メッセージを一度に 200 を超えるユーザー、または 1 日に 1 万を超える受信者に送信するか、1 分あたり 30 件を超えるメッセージを送信するように、構成されています。
- ワークフローを実行すると、メール メッセージは送信されず、ユーザーは次のような動作に気付くはずです。
    - プラットフォームの種類に SharePoint 2013 を使用するワークフローでは、[**ワークフローの状態**] ページを参照します。 [ワークフローの状態] ページで、[**内部の状態**] は [**開始済み**] に設定され、情報の吹き出しには "**受信者に送信できません**" と表示されます。

この問題を回避するには、[Exchange Online の送信者制限](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)を超過せずにメール メッセージを送信するようにワークフローを構成します。 たとえば、ワークフロー内で一時停止を使用したり、メールを Microsoft 365 グループ、配布グループ、またはメールが有効なセキュリティ グループに送信したり、一度にメッセージを送信する相手を 200 人未満の受信者にしたりします。


詳細については、以下の[記事](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)をご覧ください。

## <a name="related-topics"></a>関連項目
- [フローを作成する](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint and Flow (SharePoint と Flow)](https://flow.microsoft.com/blog/sharepoint-and-flow/) 