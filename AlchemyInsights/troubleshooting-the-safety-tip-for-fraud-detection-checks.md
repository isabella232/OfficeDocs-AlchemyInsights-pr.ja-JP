---
title: トラブルシューティングの不正行為を検出するための安全性のヒントをチェックします。
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
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29658120"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="18dec-102">トラブルシューティングの不正行為を検出するための安全性のヒントをチェックします。</span><span class="sxs-lookup"><span data-stu-id="18dec-102">Troubleshooting the safety tip for fraud detection checks</span></span>



<span data-ttu-id="18dec-p101">場合は、安全性のヒントを取得するは、送信者、不正行為の検出の確認に失敗しましたし、者として表示される場合がありますできません」、DKIM や SPF のいずれかの認証チェックに合格するのには、送信者が失敗しました。自体を承認するために送信者には、これを解決する最善の方法です。場合は、代わりに送信者が送信すると、送信者の IP アドレスを SPF レコードに追加することによってそれらを承認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="18dec-p101">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks. The best method to resolve this is for the sender to authorize themselves. If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="18dec-106">詳細情報の[確認トラブルシューティングの不正行為を検出するための赤の (疑わしい) 安全性のヒント](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="18dec-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="18dec-107">役立つその他のいくつかのリンクを以下に示します。</span><span class="sxs-lookup"><span data-stu-id="18dec-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="18dec-108">Office 365 が送信者ポリシー フレームワーク (SPF) を使用して、スプーフィングを防止する方法</span><span class="sxs-lookup"><span data-stu-id="18dec-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [<span data-ttu-id="18dec-109">スプーフィングを防止するために Office 365 で SPF を設定する</span><span class="sxs-lookup"><span data-stu-id="18dec-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

