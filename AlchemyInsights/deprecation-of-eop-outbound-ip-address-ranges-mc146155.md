---
title: 1065 EOP 送信 IP アドレスの範囲の廃止 MC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031267"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>EOP 送信 IP アドレスの範囲の廃止

オンプレミスまたは外部の送信先へのメール フローを中断する可能性があると考えられる問題が組織に見つかりました (2018 年 10 月 26 日までに修正されていない場合)。以前にお知らせしたように、IP アドレス範囲の管理を簡素化する目的で、Microsoft 365 外部の送信元または送信先とメールを送受信するために使用される Exchange Online Protection (EOP) の IP アドレス範囲を統合することを Microsoft は検討しています。Microsoft の分析によると、ユーザーがメール フロー コネクタで構成している外部メールの送信元または送信先の 1 つまたは複数が[ここ](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)に示す IP アドレス範囲からの接続を受け入れません。

10 月 26 日になる前に、そのような送信元と送信先で、すべての[公開されている EOP IP アドレス](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)との送受信接続を受け入れるようにしてください。

この変更に関する詳細については、メッセージ センターの投稿である [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155)、[MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)、[MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274) をお読みください。

**注**: 以前、エンドポイントの更新に HTML、XML、RSS 経由の IP または URL 公開を使用した場合、そのような種類の更新を自動化するための新しい Web サービスに移行する必要もあります。詳細については、「[Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)」(Microsoft 365 エンドポイント カテゴリ、および Microsoft 365 IP アドレスと URL の Web サービス) を参照してください。
