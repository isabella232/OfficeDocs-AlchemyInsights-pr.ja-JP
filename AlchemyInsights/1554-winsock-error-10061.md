---
title: 1554 Winsock エラー 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 96a9cfd11941158ddf13655c74974e3eb800e570
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28297413"
---
# <a name="winsock-error-10061"></a>Winsock エラー 10061

このエラー コードは、Office 365 がターゲット ・ ホストとの TCP ソケット (接続) を確立できなかったことを意味します。このエラーの最も一般的な原因は、ファイアウォールの構成に問題です。問題を修正するのには、これらの設定を確認します。
  
- ファイアウォールの設定と[Office 365 の Url と IP アドレスの範囲](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)内の情報を確認します。
    
- エラーが Exchange オンライン保護 (EOP) に固有の場合は、する必要があります以前に通知して[Exchange のオンライン保護の IP アドレス](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)に変更します。
    
- インターネット サービス プロバイダー (ISP) がポートをブロックされていないことを確認します。
    
- コネクタのスマート ホストとターゲット ・ サーバーの設定を確認します。
    
Office 365 がこの方法で*着信*接続をブロックしないことに注意してください。 
  

