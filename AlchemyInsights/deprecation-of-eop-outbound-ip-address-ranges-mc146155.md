---
title: 1065 EOP 送信 IP アドレスの範囲の廃止 MC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806800"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="c15cb-102">EOP 送信 IP アドレスの範囲の廃止</span><span class="sxs-lookup"><span data-stu-id="c15cb-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="c15cb-p101">オンプレミスまたは外部の送信先へのメール フローを中断する可能性があると考えられる問題が組織に見つかりました (2018 年 10 月 26 日までに修正されていない場合)。以前にお知らせしたように、IP アドレス範囲の管理を簡素化する目的で、Microsoft 365 外部の送信元または送信先とメールを送受信するために使用される Exchange Online Protection (EOP) の IP アドレス範囲を統合することを Microsoft は検討しています。Microsoft の分析によると、ユーザーがメール フロー コネクタで構成している外部メールの送信元または送信先の 1 つまたは複数が[ここ](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)に示す IP アドレス範囲からの接続を受け入れません。</span><span class="sxs-lookup"><span data-stu-id="c15cb-p101">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations. As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365. Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="c15cb-106">10 月 26 日になる前に、そのような送信元と送信先で、すべての[公開されている EOP IP アドレス](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)との送受信接続を受け入れるようにしてください。</span><span class="sxs-lookup"><span data-stu-id="c15cb-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="c15cb-107">この変更に関する詳細については、メッセージ センターの投稿である [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155)、[MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)、[MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274) をお読みください。</span><span class="sxs-lookup"><span data-stu-id="c15cb-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="c15cb-p102">**注**: 以前、エンドポイントの更新に HTML、XML、RSS 経由の IP または URL 公開を使用した場合、そのような種類の更新を自動化するための新しい Web サービスに移行する必要もあります。詳細については、「[Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)」(Microsoft 365 エンドポイント カテゴリ、および Microsoft 365 IP アドレスと URL の Web サービス) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c15cb-p102">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates. For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
