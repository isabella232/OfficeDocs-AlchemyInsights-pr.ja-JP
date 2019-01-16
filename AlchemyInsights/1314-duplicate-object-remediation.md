---
title: 1314 オブジェクトの複製の問題解決
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: b8543b7e-fd00-4b3c-be68-a1758b8caf78
ms.openlocfilehash: 7dc629afcad312be80f47299d81ed320a11aa40c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28297552"
---
# <a name="duplicate-object-synchronization-errors"></a><span data-ttu-id="6012b-102">重複したオブジェクトの同期エラー</span><span class="sxs-lookup"><span data-stu-id="6012b-102">Duplicate object synchronization errors</span></span>

<span data-ttu-id="6012b-103">場合は、同期中に次のエラーのいずれかが表示されます。</span><span class="sxs-lookup"><span data-stu-id="6012b-103">If you receive one of the following errors during a synchronization:</span></span>
  
- <span data-ttu-id="6012b-104">同じプロキシ アドレスを使用して同期されたオブジェクトは、Microsoft Online Services ディレクトリに既に存在します。</span><span class="sxs-lookup"><span data-stu-id="6012b-104">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>
    
- <span data-ttu-id="6012b-105">UserPrincipalName のようなメッセージです。</span><span class="sxs-lookup"><span data-stu-id="6012b-105">A similar message for UserPrincipalName.</span></span>
    
<span data-ttu-id="6012b-p101">重複するオブジェクトのエラーを解決するのには、新しい AADConnect 健康診断を使用します。詳細についてを参照してください[診断と重複している属性の同期エラーを改善する](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors)です。</span><span class="sxs-lookup"><span data-stu-id="6012b-p101">use the new AADConnect Health diagnostic to resolve duplicate object errors. For more information, see [Diagnose and remediate duplicated attribute sync errors](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-diagnose-sync-errors).</span></span>
  

