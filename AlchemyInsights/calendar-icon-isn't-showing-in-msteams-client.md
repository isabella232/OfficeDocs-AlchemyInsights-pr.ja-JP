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
ms.openlocfilehash: edd6b4a2d94b03cf4ae7bf3a8d6332ed94a7e8263aba9df1f9588eecbd0ce05a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54120009"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>Microsoft Teams クライアントに予定表アイコンが表示されない

Teams の **[予定表]** タブでは、Exchange Web サービスを使用して Exchange メールボックスにアクセスする必要があります。 Exchange メールボックスは、オンラインまたはオンプレミスである可能性があります。 オンライン ユーザーで **[予定表]** タブが表示されない場合には、[Exchange Online メールボックスのライセンスがあり、メールボックスが有効になっている](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes)ことを確認してください。 ユーザーがオンプレミスに属している場合、ハイブリッド構成が正常であることを確認する必要があります。 [ハイブリッド構成ウィザード](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent)を使用して、トラブルシューティングします。 [Teams では Exchange 2016 CU3 以上](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)が必要であることに注意してください。

詳細とトラブルシューティング手順の詳細については、「[Microsoft Teams と Exchange Server の相互作用の問題のトラブルシューティング](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue)」を参照してください。
