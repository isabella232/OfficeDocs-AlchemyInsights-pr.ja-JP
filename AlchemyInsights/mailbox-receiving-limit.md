---
title: メールボックス受信制限の実施
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/31/2021
ms.locfileid: "59316393"
---
# <a name="mailbox-receiving-limit-enforcement"></a>メールボックス受信制限の実施

Microsoft は最近、メールボックスごとのしきい値である 1 時間あたり 3600 メッセージの適用を開始しました。 詳細については、「[Exchange Online の制限](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits)」をご覧ください。 1 時間以内に 3600 を超えるメッセージを受信する Microsoft 365 メールボックスは、次の 60 分間抑制されます。 

さらに、Microsoft 365 メールボックスが特定の送信者から受信したメッセージをブロックする送信者と受信者のペア (SRP) の制限が適用されます。 1 人の送信者が合計しきい値の 33% 以上、つまりローリング時間あたり 1200 メッセージを特定の受信者に送信すると、SRP 制限が適用され、メールボックスはその送信者からのメッセージを受け入れなくなります。 次の点に注意してください。

- この制限は、他のテナント、オンプレミス、またはインターネット送信者から受信したメールに適用されます。
- メールボックスへのメール配信は、次の 60 分間ブロックされます。 
- これらのメールボックスへの送信者は、メールボックスが最大配信しきい値を超えたことを示す配信不能レポート (5.2.121 または 5.2.122) を受信します。 テナント内 (同じテナント内のメール) は引き続き配信されます。
- SRP 制限が適用されると、受信メールボックスは他の送信者からのメッセージを引き続き受け入れます。

管理者は、Exchange 管理センターの "受信制限を超えるメールボックス" と呼ばれる新しいレポートと分析情報にアクセスすることで、現在のメールボックス アクティビティを監視できます。 分析情報は、テナントに問題のあるメールボックスがある場合にのみ表示されますが、レポートは常にダッシュボードに表示され、テナントに問題のあるメールボックスがない限り空になります。

分析情報受信制限の詳細については、「[最新の EAC での受信制限を超えるメールボックスについての分析情報](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights)」を参照してください。

受信制限超過レポートの詳細については、「[最新の EAC での受信制限を超えるメールボックスについてのレポート](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report)」を参照してください。