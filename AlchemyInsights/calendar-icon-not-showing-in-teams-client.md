---
title: Teams クライアントに予定表アイコンが表示されない
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/24/2020
ms.locfileid: "42935342"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Teams クライアントに予定表アイコンが表示されない

Teams の [予定表] タブでは、Exchange Web サービスを使用して Exchange メールボックスにアクセスする必要があります。 Exchange メールボックスは、オンラインまたはオンプレミスである可能性があります。 オンライン ユーザーで [予定表] タブが表示されない場合には、[Exchange Online メールボックスのライセンスがあり、メールボックスが有効になっている](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes)ことを確認してください。

Exchange Online の有効なメールボックスがあるものの [予定表] タブが表示されない場合には、ネットワークの問題が発生している可能性があります。 関係するユーザーに対して [Microsoft リモート接続アナライザー](https://testconnectivity.microsoft.com/)を使用して、**Microsoft Exchange Web サービス接続テスト**を実行します。

最後に、[Teams のアプリ - アプリのセットアップ ポリシー](https://admin.teams.microsoft.com/policies/app-setup)を調べて、予定表アプリがユーザーに適用されているポリシー (多くの場合は **(組織全体の既定) グローバル)** から削除されていないことを確認します。

ユーザーがオンプレミスに属している場合、ハイブリッド構成の正常性を確認する必要があります。 [ハイブリッド構成ウィザード](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent)を使用して、トラブルシューティングします。

[Teams では Exchange 2016 CU3 以上](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)が必要であることに注意してください。
