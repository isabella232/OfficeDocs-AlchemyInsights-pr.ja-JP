---
title: 1554 Winsock エラー 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 9331a6c2b6e92a66fb97daf7dc5655ec320cba0f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "29903106"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="b0f84-102">Winsock エラー 10061</span><span class="sxs-lookup"><span data-stu-id="b0f84-102">Winsock error 10061</span></span>

<span data-ttu-id="b0f84-p101">このエラー コードは、Office 365 がターゲット ホストとの TCP ソケット (接続) を確立できなかったことを示しています。このエラーの最も一般的な原因は、ファイアウォールの構成上の問題です。この問題を修正するのには、次の設定を確認してください。</span><span class="sxs-lookup"><span data-stu-id="b0f84-p101">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="b0f84-106">「[Office 365 の URL と IP アドレスの範囲](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)」の情報を参照して、ファイアウォール構成を確認します。</span><span class="sxs-lookup"><span data-stu-id="b0f84-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="b0f84-107">エラーが Exchange Online Protection (EOP) に固有のものである場合は、[Exchange Online Protection の IP アドレス](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)の変更に関する通知を既に受け取っているはずです。</span><span class="sxs-lookup"><span data-stu-id="b0f84-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="b0f84-108">インターネット サービス プロバイダー (ISP) がポートをブロックしていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="b0f84-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="b0f84-109">コネクタでスマート ホストとターゲット サーバーの設定を確認します。</span><span class="sxs-lookup"><span data-stu-id="b0f84-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="b0f84-110">なお、Office 365 がこのような仕方で  *受信*  接続をブロックすることはありません。</span><span class="sxs-lookup"><span data-stu-id="b0f84-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

