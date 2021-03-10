---
title: ラベルの優先度 (順序の問題)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7455"
- "9000181"
ms.openlocfilehash: 2ed92401399466e41349066cb4c9250c4da3c2c9
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527876"
---
# <a name="label-priority-order-matters"></a><span data-ttu-id="70dfa-102">ラベルの優先度 (順序の問題)</span><span class="sxs-lookup"><span data-stu-id="70dfa-102">Label priority (order matters)</span></span>

<span data-ttu-id="70dfa-103">秘密度ラベルを管理センターで作成すると、そのラベルは **[ラベル]** ページの **[秘密度]** タブにあるリストに表示されます。</span><span class="sxs-lookup"><span data-stu-id="70dfa-103">When you create sensitivity labels in the admin center, they appear in a list on the **Sensitivity** tab on the **Labels** page.</span></span> <span data-ttu-id="70dfa-104">このリストでは、ラベルの順序が重要になります。その理由は、この順序がラベルの優先度を反映しているためです。</span><span class="sxs-lookup"><span data-stu-id="70dfa-104">In this list, the order of the labels is important, because it reflects their priority.</span></span> <span data-ttu-id="70dfa-105">厳密な秘密度ラベル (「極秘」など) はリストの **下側** に表示されるようにして、最も厳密でない秘密度ラベル (「公開」など) はリストの **上側** に表示されるようにします。</span><span class="sxs-lookup"><span data-stu-id="70dfa-105">You want your restrictive sensitivity label, such as **Highly Confidential**, to appear at the bottom of the list, and your least restrictive sensitivity label, such as **Public**, to appear at the top.</span></span>

<span data-ttu-id="70dfa-106">各ドキュメントまたはメールに適用できる秘密度ラベルは 1 つだけです。</span><span class="sxs-lookup"><span data-stu-id="70dfa-106">You can apply just one sensitivity label to a document or email.</span></span> <span data-ttu-id="70dfa-107">ラベルの分類を低く変更する場合の正当性を示すようユーザーに要求するオプションを選択する場合は、より低い分類はこの一覧の順序によって特定されます。</span><span class="sxs-lookup"><span data-stu-id="70dfa-107">If you set an option that requires your users to provide a justification for changing a label to a lower classification, the order of this list identifies the lower classifications.</span></span>

<span data-ttu-id="70dfa-108">サブラベルの順序は、[自動ラベル付け](https://docs.microsoft.com/microsoft-365/compliance/apply-sensitivity-label-automatically)を介して行われます。</span><span class="sxs-lookup"><span data-stu-id="70dfa-108">The ordering of sublabels is done through [automatic labeling](https://docs.microsoft.com/microsoft-365/compliance/apply-sensitivity-label-automatically).</span></span> <span data-ttu-id="70dfa-109">ラベルが自動的に適用されるように構成した場合、またはラベルが推奨されるように構成した場合、複数のラベルにまたがる複数の一致が検出される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="70dfa-109">When you configure labels to be applied automatically or as a recommendation, multiple matches can result for more than one label.</span></span> <span data-ttu-id="70dfa-110">詳細については、「[ラベルの優先度 (順序の問題)](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="70dfa-110">For more information, see [Label priority (order matters)](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span></span>