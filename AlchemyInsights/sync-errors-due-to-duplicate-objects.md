---
title: 902 (重複するオブジェクトに起因する同期エラー)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 06cd582c30a59a94ee117728bd5daebecca77bc8
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758000"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="5b060-102">重複するオブジェクトに起因する同期エラー</span><span class="sxs-lookup"><span data-stu-id="5b060-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="5b060-103">ディレクトリ同期が終了したときに、次のいずれかのエラー メッセージが表示される場合があります。</span><span class="sxs-lookup"><span data-stu-id="5b060-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>

- <span data-ttu-id="5b060-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory. (このオブジェクトに関連付けられた次の属性値はローカル ディレクトリで既に他のオブジェクトに関連付けられているため、Microsoft Online Services でこのオブジェクトを更新できません。)</span><span class="sxs-lookup"><span data-stu-id="5b060-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="5b060-105">同じプロキシ アドレスを持つ同期済みオブジェクトが Microsoft Online Services ディレクトリ内に既に存在します。</span><span class="sxs-lookup"><span data-stu-id="5b060-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="5b060-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName. (このオブジェクトに関連付けられた属性値 UserPrincipalName は、ローカル ディレクトリ サービスの他のオブジェクトに既に関連付けられているため、このオブジェクトを更新できません。)</span><span class="sxs-lookup"><span data-stu-id="5b060-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="5b060-107">問題を特定して修正するには、[IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832) をダウンロードして実行します。</span><span class="sxs-lookup"><span data-stu-id="5b060-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="5b060-108">詳細については、「[KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5b060-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
