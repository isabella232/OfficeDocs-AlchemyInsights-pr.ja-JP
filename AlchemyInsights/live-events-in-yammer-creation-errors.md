---
title: Yammer 作成エラーのライブ イベント
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
- "9002495"
- "5112"
ms.openlocfilehash: eb1ef3712038827beafc8eb520f9793da5f357d728e8250c16d88a99b8b5fe20
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114933"
---
# <a name="live-events-in-yammer-creation-errors"></a>Yammer 作成エラーのライブ イベント

**Yammer ライブ イベントの作成**

Yammer には、常にライブ イベントの作成をするオプションが表示されます。 場合によっては、ユーザーがライブ イベント作成の前提条件を満たしていないことがあり、ユーザーが作成しようとしたときにエラーが表示されることがあります。 以下では、この問題の一般的な理由について説明し、エンドユーザーが問題を解決する方法を示します。

**ライブ イベントを作成できるユーザー**
- Office 365 Enterprise E1、E3、E5 のいずれかのライセンス、または Office 365 A3 または A5 ライセンスがある。
- Microsoft Teams 管理センターでのライブ イベントを作成するためのアクセスを許可されている。
- Microsoft Stream でのライブ イベントを作成するためのアクセスを許可されている (外部へのブロードキャストのアプリまたはデバイスを使用して作成されたイベントの場合)。
- 組織内の完全なチーム メンバーシップがある (ゲストや別の組織のメンバーは不可)。
- プライベート会議のスケジュール、画面共有、IP ビデオの共有は、Teams の会議ポリシーでは有効になります。

**ライブ イベントの作成のポリシー**

Yammer は、ストリーム用の Office 365 テナントに設定されているライブ イベントポリシーに従います。 既定では、組織内のすべてのユーザーがライブ イベントを作成できます。 管理者が[この設定を変更すると、ユーザーがライブ イベントを作成できなくなる可能性があり ます](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating)。 ユーザーがポリシーエラーを受信した場合、ライブ イベントを作成する権限があることを確認することが重要です。
