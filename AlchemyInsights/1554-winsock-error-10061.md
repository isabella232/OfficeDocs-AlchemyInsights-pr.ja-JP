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
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29477157"
---
# <a name="winsock-error-10061"></a>Winsock エラー 10061

このエラー コードは、Office 365 がターゲット ホストとの TCP ソケット (接続) を確立できなかったことを示しています。このエラーの最も一般的な原因は、ファイアウォールの構成上の問題です。この問題を修正するのには、次の設定を確認してください。
  
- 「[Office 365 の URL と IP アドレスの範囲](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)」の情報を参照して、ファイアウォール構成を確認します。
    
- エラーが Exchange Online Protection (EOP) に固有のものである場合は、[Exchange Online Protection の IP アドレス](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)の変更に関する通知を既に受け取っているはずです。
    
- インターネット サービス プロバイダー (ISP) がポートをブロックしていないことを確認します。
    
- コネクタでスマート ホストとターゲット サーバーの設定を確認します。
    
なお、Office 365 がこのような仕方で  *受信*  接続をブロックすることはありません。 
  

