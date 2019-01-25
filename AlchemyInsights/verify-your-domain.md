---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: d37cdae616fabd2813dc7c8074e94b05f0391d20
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29477420"
---
# <a name="verify-your-domain"></a><span data-ttu-id="66b12-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="66b12-102">Verify your domain</span></span>

 <span data-ttu-id="66b12-103">**レコードをインターネット経由で更新していない可能性があります。**</span><span class="sxs-lookup"><span data-stu-id="66b12-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="66b12-104">通常ほんの数分、新しいレコードを表示できるのですが、場合によってはかかることがいくつかの時間の長さです。</span><span class="sxs-lookup"><span data-stu-id="66b12-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="66b12-p101">既に長い間を待機している場合、は、コピーし、TXT 確認レコードを DNS ホストの正確な値を貼り付けることを再確認してください。1 つの一般的な問題が含まれていません、"MS ="のレコードの一部です。必要があることも!</span><span class="sxs-lookup"><span data-stu-id="66b12-p101">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host. One common issue is not including the "MS=" part of the record. We need that too!</span></span>
    
- <span data-ttu-id="66b12-p102">一部の DNS ホストがある場合 (DNS レコードが格納されますが)、ゾーン ファイルを保存するのには余分な手順を実行するため、インターネット経由で更新されます。Office 365 は、表示し、レコードを検証するため、変更内容が保存されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="66b12-p102">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet. Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
    

