---
title: 1065 EOP 送信 IP アドレスの範囲の廃止 MC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 17beb1722142d94ea05b67ce5ed1f20f8b11375c
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404826"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="4daaf-102">EOP 送信 IP アドレスの範囲の廃止</span><span class="sxs-lookup"><span data-stu-id="4daaf-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="4daaf-p101">オンプレミスまたは外部の送信先へのメール フローを中断する可能性があると考えられる問題が組織に見つかりました (2018 年 10 月 26 日までに修正されていない場合)。以前にお知らせしたように、IP アドレス範囲の管理を簡素化する目的で、Office 365 の外とメールを送受信するために使用される Exchange Online Protection (EOP) の IP アドレス範囲を統合することを Microsoft は検討しています。Microsoft の分析によると、ユーザーがメール フロー コネクタで構成している外部メールの送信元または送信先の 1 つまたは複数が[ここ](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)に示す IP アドレス範囲からの接続を受け入れません。</span><span class="sxs-lookup"><span data-stu-id="4daaf-p101">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations. As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365. Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="4daaf-106">10 月 26 日になる前に、そのような送信元と送信先で、すべての[公開されている EOP IP アドレス](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)との送受信接続を受け入れるようにしてください。</span><span class="sxs-lookup"><span data-stu-id="4daaf-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="4daaf-107">この変更に関する詳細については、メッセージ センターの投稿である [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155)、[MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)、[MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274) をお読みください。</span><span class="sxs-lookup"><span data-stu-id="4daaf-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="4daaf-p102">**注**: 以前、エンドポイントの更新に HTML、XML、RSS 経由の IP または URL 公開を使用した場合、そのような種類の更新を自動化するための新しい Web サービスに移行する必要もあります。詳細については、「[Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)」 (Office 365 エンドポイント カテゴリ、および Office 365 IP アドレスと URL の Web サービス) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4daaf-p102">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates. For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
