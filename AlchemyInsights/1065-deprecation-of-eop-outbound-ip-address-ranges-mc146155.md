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
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29477334"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="2f263-102">送信 IP アドレスの範囲の EOP の廃止</span><span class="sxs-lookup"><span data-stu-id="2f263-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="2f263-p101">(修正されない場合は、2018 年 10 月 26 日によって) は、設置や外部の宛先にメールの流れを壊す可能性がある組織に潜在的な問題を検出しましたしました。IP アドレス範囲の管理を簡素化する以前に伝達として Office 365 以外でメールの送受信に使用される Exchange オンライン保護 (EOP) の IP アドレスの範囲に統合されています。マイクロソフトの分析では、1 つまたは複数の電子メールを外部ソースまたは宛先のメール フローのコネクタに設定されているが、IP アドレスの範囲に示すように[ここ](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)からの接続を受け付けていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="2f263-p101">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations. As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365. Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="2f263-106">これらのソースと宛先は[EOP の IP アドレスを発行する](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)すべてのとの間の接続を受け入れることを確認するのには 26 年 10 月の前に動作します。</span><span class="sxs-lookup"><span data-stu-id="2f263-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="2f263-107">この変更の詳細については、メッセージ センター [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155)、 [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)、または[MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)の投稿を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2f263-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>
  
 <span data-ttu-id="2f263-p102">**注**: エンドポイントの更新プログラムの HTML、XML、および RSS を使用して IP または URL の発行を使用していた場合もする必要がありますに移行するこれらの種類の更新を自動化するための新しい web サービスです。詳細については、 [Office 365 エンドポイントのカテゴリと Office 365 の IP アドレス、および web サービスの URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2f263-p102">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates. For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
  

