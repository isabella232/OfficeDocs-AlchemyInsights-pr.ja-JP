---
title: Teams クライアントに予定表アイコンが表示されない
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819958"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Teams クライアントに予定表アイコンが表示されない

Teams の [予定表] タブでは、Exchange Web サービスを使用して Exchange メールボックスにアクセスする必要があります。 Exchange メールボックスは、オンラインまたはオンプレミスである可能性があります。 オンライン ユーザーで [予定表] タブが表示されない場合には、[Exchange Online メールボックスのライセンスがあり、メールボックスが有効になっている](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes)ことを確認してください。

Exchange Online の有効なメールボックスがあるものの [予定表] タブが表示されない場合には、ネットワークの問題が発生している可能性があります。 関係するユーザーに対して [Microsoft リモート接続アナライザー](https://testconnectivity.microsoft.com/)を使用して、**Microsoft Exchange Web サービス接続テスト** を実行します。

最後に、[Teams のアプリ - アプリのセットアップ ポリシー](https://admin.teams.microsoft.com/policies/app-setup)を調べて、予定表アプリがユーザーに適用されているポリシー (多くの場合は **(組織全体の既定) グローバル)** から削除されていないことを確認します。

ユーザーがオンプレミスに属している場合、ハイブリッド構成の正常性を確認する必要があります。 [ハイブリッド構成ウィザード](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent)を使用して、トラブルシューティングします。

[Teams では Exchange 2016 CU3 以上](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)が必要であることに注意してください。
