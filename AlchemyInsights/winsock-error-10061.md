---
title: 1554 Winsock エラー 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698867"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="48013-102">Winsock エラー 10061</span><span class="sxs-lookup"><span data-stu-id="48013-102">Winsock error 10061</span></span>

<span data-ttu-id="48013-p101">このエラー コードは、Microsoft がターゲット ホストとの TCP ソケット (接続) を確立できなかったことを示しています。このエラーの最も一般的な原因は、ファイアウォールの構成上の問題です。この問題を修正するのには、次の設定を確認してください。</span><span class="sxs-lookup"><span data-stu-id="48013-p101">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>

- <span data-ttu-id="48013-106">「[Microsoft 365 の URL と IP アドレスの範囲](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)」の情報を参照して、ファイアウォール構成を確認します。</span><span class="sxs-lookup"><span data-stu-id="48013-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="48013-107">エラーが Exchange Online Protection (EOP) に固有のものである場合は、[Exchange Online Protection の IP アドレス](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)の変更に関する通知を既に受け取っているはずです。</span><span class="sxs-lookup"><span data-stu-id="48013-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="48013-108">インターネット サービス プロバイダー (ISP) がポートをブロックしていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="48013-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="48013-109">コネクタでスマート ホストとターゲット サーバーの設定を確認します。</span><span class="sxs-lookup"><span data-stu-id="48013-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="48013-110">Microsoft 365 はこの方法で*着信*接続をブロックしないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="48013-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
