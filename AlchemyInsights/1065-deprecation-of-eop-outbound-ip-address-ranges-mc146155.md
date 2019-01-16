---
title: 1065 廃止の EOP 送信 IP アドレス rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: ec87141ffaa2fa3484620a9b52851e3e92f20b6b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28297555"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>送信 IP アドレスの範囲の EOP の廃止

(修正されない場合は、2018 年 10 月 26 日によって) は、設置や外部の宛先にメールの流れを壊す可能性がある組織に潜在的な問題を検出しましたしました。IP アドレス範囲の管理を簡素化する以前に伝達として Office 365 以外でメールの送受信に使用される Exchange オンライン保護 (EOP) の IP アドレスの範囲に統合されています。マイクロソフトの分析では、1 つまたは複数の電子メールを外部ソースまたは宛先のメール フローのコネクタに設定されているが、IP アドレスの範囲に示すように[ここ](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)からの接続を受け付けていないことを示します。
  
これらのソースと宛先は[EOP の IP アドレスを発行する](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)すべてのとの間の接続を受け入れることを確認するのには 26 年 10 月の前に動作します。
  
この変更の詳細については、メッセージ センター [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155)、 [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)、または[MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)の投稿を参照してください。
  
 **注**: エンドポイントの更新プログラムの HTML、XML、および RSS を使用して IP または URL の発行を使用していた場合もする必要がありますに移行するこれらの種類の更新を自動化するための新しい web サービスです。詳細については、 [Office 365 エンドポイントのカテゴリと Office 365 の IP アドレス、および web サービスの URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)を参照してください。
  

