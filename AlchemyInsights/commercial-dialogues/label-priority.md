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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751272"
---
# <a name="label-priority-order-matters"></a>ラベルの優先度 (順序の問題)

秘密度ラベルを管理センターで作成すると、そのラベルは **[ラベル]** ページの **[秘密度]** タブにあるリストに表示されます。 このリストでは、ラベルの順序が重要になります。その理由は、この順序がラベルの優先度を反映しているためです。 厳密な秘密度ラベル (「極秘」など) はリストの **下側** に表示されるようにして、最も厳密でない秘密度ラベル (「公開」など) はリストの **上側** に表示されるようにします。

各ドキュメントまたはメールに適用できる秘密度ラベルは 1 つだけです。 ラベルの分類を低く変更する場合の正当性を示すようユーザーに要求するオプションを選択する場合は、より低い分類はこの一覧の順序によって特定されます。

サブラベルの順序は、[自動ラベル付け](https://docs.microsoft.com/microsoft-365/compliance/apply-sensitivity-label-automatically)を介して行われます。 ラベルが自動的に適用されるように構成した場合、またはラベルが推奨されるように構成した場合、複数のラベルにまたがる複数の一致が検出される可能性があります。 詳細については、「[ラベルの優先度 (順序の問題)](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)」を参照してください。