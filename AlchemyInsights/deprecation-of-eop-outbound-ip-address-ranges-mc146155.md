---
title: 1065 EOP 送信 IP アドレスの範囲の廃止 MC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704602"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>EOP 送信 IP アドレスの範囲の廃止

組織で問題が発生する可能性があります (10 月の26th によって修正されていない場合、2018)、社内または外部の宛先にメールフローが中断する可能性があります。前にも説明したように、IP アドレス範囲の管理を簡素化するために、Microsoft 365 の外部で電子メールを送受信するために使用される Exchange Online Protection (EOP) IP アドレス範囲を統合しています。この分析では、メールフローコネクタで構成した外部電子メールの送信元または送信先の1つ以上が、[ここ](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)に示されている IP アドレスの範囲からの接続を受け付けないことを示しています。

10 月 26 日になる前に、そのような送信元と送信先で、すべての[公開されている EOP IP アドレス](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)との送受信接続を受け入れるようにしてください。

この変更に関する詳細については、メッセージ センターの投稿である [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155)、[MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)、[MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274) をお読みください。

**注**: エンドポイントの更新のために、HTML、XML、RSS 経由で IP または URL の公開を以前に使用していた場合は、これらの種類の更新プログラムを自動化するために新しい web サービスに移行する必要もあります。詳細については、「 [microsoft 365 エンドポイントカテゴリ」および「microsoft 365 IP アドレスと URL web サービス](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)」を参照してください。
