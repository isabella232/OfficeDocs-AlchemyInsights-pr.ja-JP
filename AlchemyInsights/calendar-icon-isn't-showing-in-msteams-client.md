---
title: Microsoft Teams クライアントに予定表アイコンが表示されない
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584211"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>Microsoft Teams クライアントに予定表アイコンが表示されない

Teams の **[予定表]** タブでは、Exchange Web サービスを使用して Exchange メールボックスにアクセスする必要があります。 Exchange メールボックスは、オンラインまたはオンプレミスである可能性があります。 オンライン ユーザーで **[予定表]** タブが表示されない場合には、[Exchange Online メールボックスのライセンスがあり、メールボックスが有効になっている](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes)ことを確認してください。 ユーザーがオンプレミスに属している場合、ハイブリッド構成が正常であることを確認する必要があります。 [ハイブリッド構成ウィザード](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent)を使用して、トラブルシューティングします。 [Teams では Exchange 2016 CU3 以上](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)が必要であることに注意してください。

詳細とトラブルシューティング手順の詳細については、「[Microsoft Teams と Exchange Server の相互作用の問題のトラブルシューティング](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue)」を参照してください。
