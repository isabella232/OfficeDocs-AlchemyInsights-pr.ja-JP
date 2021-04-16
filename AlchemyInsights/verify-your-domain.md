---
title: ドメインの検証
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51770996"
---
# <a name="verify-your-domain"></a><span data-ttu-id="c2389-102">ドメインの検証</span><span class="sxs-lookup"><span data-stu-id="c2389-102">Verify your domain</span></span>

 <span data-ttu-id="c2389-103">**レコードがインターネット経由で更新されていない可能性があります。**</span><span class="sxs-lookup"><span data-stu-id="c2389-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="c2389-104">通常、ユーザーへの新しいレコードの表示には数分しかかかりませんが、場合によっては、数時間かかることもあります。</span><span class="sxs-lookup"><span data-stu-id="c2389-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="c2389-p101">既にその時間は待っている場合、DNS ホストで正確な値をコピーし、TXT 検証レコードに貼り付けたことを二重に確認してください。よくある原因の 1 つとして、レコードの「MS=」部分が含められていないことがあります。この部分も含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="c2389-p101">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host. One common issue is not including the "MS=" part of the record. We need that too!</span></span>

- <span data-ttu-id="c2389-p102">DNS ホストによっては、インターネット全体で更新されるようにゾーン ファイル (DNS レコードが保存されているファイル) を保存するという作業も必要になります。Microsoft がレコードを表示し、確認できるように、変更内容は必ず保存してください。</span><span class="sxs-lookup"><span data-stu-id="c2389-p102">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet. Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
