---
title: 1554 Winsock エラー 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766174"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="378ff-102">Winsock エラー 10061</span><span class="sxs-lookup"><span data-stu-id="378ff-102">Winsock error 10061</span></span>

<span data-ttu-id="378ff-p101">このエラー コードは、Microsoft がターゲット ホストとの TCP ソケット (接続) を確立できなかったことを示しています。このエラーの最も一般的な原因は、ファイアウォールの構成上の問題です。この問題を修正するのには、次の設定を確認してください。</span><span class="sxs-lookup"><span data-stu-id="378ff-p101">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>

- <span data-ttu-id="378ff-106">「[Microsoft 365 の URL と IP アドレスの範囲](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)」の情報を参照して、ファイアウォール構成を確認します。</span><span class="sxs-lookup"><span data-stu-id="378ff-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="378ff-107">エラーが Exchange Online Protection (EOP) に固有のものである場合は、[Exchange Online Protection の IP アドレス](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)の変更に関する通知を既に受け取っているはずです。</span><span class="sxs-lookup"><span data-stu-id="378ff-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="378ff-108">インターネット サービス プロバイダー (ISP) がポートをブロックしていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="378ff-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="378ff-109">コネクタでスマート ホストとターゲット サーバーの設定を確認します。</span><span class="sxs-lookup"><span data-stu-id="378ff-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="378ff-110">Microsoft 365 はこの方法で*着信*接続をブロックしないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="378ff-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
