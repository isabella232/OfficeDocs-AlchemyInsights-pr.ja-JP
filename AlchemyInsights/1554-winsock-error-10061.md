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
# <a name="winsock-error-10061"></a><span data-ttu-id="2e3e5-102">Winsock エラー 10061</span><span class="sxs-lookup"><span data-stu-id="2e3e5-102">Winsock error 10061</span></span>

<span data-ttu-id="2e3e5-p101">このエラー コードは、Office 365 がターゲット ・ ホストとの TCP ソケット (接続) を確立できなかったことを意味します。このエラーの最も一般的な原因は、ファイアウォールの構成に問題です。問題を修正するのには、これらの設定を確認します。</span><span class="sxs-lookup"><span data-stu-id="2e3e5-p101">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="2e3e5-106">ファイアウォールの設定と[Office 365 の Url と IP アドレスの範囲](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)内の情報を確認します。</span><span class="sxs-lookup"><span data-stu-id="2e3e5-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="2e3e5-107">エラーが Exchange オンライン保護 (EOP) に固有の場合は、する必要があります以前に通知して[Exchange のオンライン保護の IP アドレス](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)に変更します。</span><span class="sxs-lookup"><span data-stu-id="2e3e5-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="2e3e5-108">インターネット サービス プロバイダー (ISP) がポートをブロックされていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="2e3e5-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="2e3e5-109">コネクタのスマート ホストとターゲット ・ サーバーの設定を確認します。</span><span class="sxs-lookup"><span data-stu-id="2e3e5-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="2e3e5-110">Office 365 がこの方法で*着信*接続をブロックしないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="2e3e5-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

