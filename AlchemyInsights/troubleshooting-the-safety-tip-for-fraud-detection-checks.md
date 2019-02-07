---
title: 不正検出チェックの安全性のヒントのトラブルシューティングを行う
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 06a0b5b8d29052e6033de5938b8ea67ceabc9848
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29658120"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="5670a-102">不正検出チェックの安全性のヒントのトラブルシューティングを行う</span><span class="sxs-lookup"><span data-stu-id="5670a-102">Troubleshooting the safety tip for fraud detection checks</span></span>



<span data-ttu-id="5670a-p101">「送信者不正検出チェックに合格せず、なりすましの可能性がある」ことを示す安全性のヒントが表示される場合には、送信者は DKIM または SPF 認証チェックに合格しませんでした。この問題を解決する最善の方法は、送信者自身が認証を受けることです。お客様に代わって送信者が送信する場合、その送信者の IP アドレスをご使用の SPF レコードに追加し、送信者を認証する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5670a-p101">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks. The best method to resolve this is for the sender to authorize themselves. If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="5670a-106">詳しくは、「[不正検出チェックの赤い (不審) 安全性のヒントに関するトラブルシューティングを行う](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="5670a-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="5670a-107">以下に役立つその他のリンクをいくつか記します。</span><span class="sxs-lookup"><span data-stu-id="5670a-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="5670a-108">Office 365 において Sender Policy Framework (SPF) を使用して、スプーフィングを防止する方法</span><span class="sxs-lookup"><span data-stu-id="5670a-108">How Office 365 uses Sender Policy Framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [<span data-ttu-id="5670a-109">スプーフィングを防止するために Office 365 で SPF を設定する</span><span class="sxs-lookup"><span data-stu-id="5670a-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

