---
title: 902 (オブジェクトの複製で発生する同期エラー)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f8db233167a5e2b2ef7290438b8e6d92d0dccb1e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29477503"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="85023-102">オブジェクトの複製のための同期エラー</span><span class="sxs-lookup"><span data-stu-id="85023-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="85023-103">ディレクトリ同期処理が完了するとに、次のエラー メッセージのいずれかが表示される場合があります。</span><span class="sxs-lookup"><span data-stu-id="85023-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>
  
- <span data-ttu-id="85023-104">このオブジェクトに関連付けられている属性は次の値をローカル ディレクトリ内の別のオブジェクトに関連付けられて既に場合があるために、Microsoft Online Services では、このオブジェクトを更新できません。</span><span class="sxs-lookup"><span data-stu-id="85023-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>
    
- <span data-ttu-id="85023-105">同じプロキシ アドレスを使用して同期されたオブジェクトは、Microsoft Online Services ディレクトリに既に存在します。</span><span class="sxs-lookup"><span data-stu-id="85023-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>
    
- <span data-ttu-id="85023-106">このオブジェクトに関連付けられている次の属性値をローカルのディレクトリ サービス内の別のオブジェクトに関連付けられていることがありますので、このオブジェクトを更新できません: UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="85023-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>
    
<span data-ttu-id="85023-107">問題の解決については、ダウンロードして、 [IdFix ディレクトリ同期エラーの修復ツール](https://www.microsoft.com/download/details.aspx?id=36832)を実行します。</span><span class="sxs-lookup"><span data-stu-id="85023-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>
  
<span data-ttu-id="85023-108">詳細については、 [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="85023-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
  

