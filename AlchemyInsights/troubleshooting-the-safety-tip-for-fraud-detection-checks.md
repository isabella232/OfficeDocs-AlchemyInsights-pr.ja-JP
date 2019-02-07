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
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>不正検出チェックの安全性のヒントのトラブルシューティングを行う



「送信者不正検出チェックに合格せず、なりすましの可能性がある」ことを示す安全性のヒントが表示される場合には、送信者は DKIM または SPF 認証チェックに合格しませんでした。この問題を解決する最善の方法は、送信者自身が認証を受けることです。お客様に代わって送信者が送信する場合、その送信者の IP アドレスをご使用の SPF レコードに追加し、送信者を認証する必要があります。
  
詳しくは、「[不正検出チェックの赤い (不審) 安全性のヒントに関するトラブルシューティングを行う](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/)」をご覧ください。 
  
以下に役立つその他のリンクをいくつか記します。
  
- [Office 365 において Sender Policy Framework (SPF) を使用して、スプーフィングを防止する方法](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [スプーフィングを防止するために Office 365 で SPF を設定する](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

