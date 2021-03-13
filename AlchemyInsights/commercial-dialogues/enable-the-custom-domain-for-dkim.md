---
title: DKIM 用のカスタム ドメインを有効にする
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 1a21101602f47dcb5c9b607d7bbccfacec00f43a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751310"
---
# <a name="enable-the-custom-domain-for-dkim"></a><span data-ttu-id="23168-102">DKIM 用のカスタム ドメインを有効にする</span><span class="sxs-lookup"><span data-stu-id="23168-102">Enable the custom domain for DKIM</span></span>

<span data-ttu-id="23168-103">カスタム ドメインの CNAME レコードを作成した後に、ドメインを有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="23168-103">After you create the CNAME records for your custom domains, you need to enable the domain.</span></span>

<span data-ttu-id="23168-104">ドメインを有効にするには、以下の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="23168-104">To enable the domain, perform the following steps:</span></span>

1. <span data-ttu-id="23168-105">[Exchange 管理センター](https://outlook.office365.com/ecp/)に移動します。</span><span class="sxs-lookup"><span data-stu-id="23168-105">Navigate to the [Exchange admin center](https://outlook.office365.com/ecp/).</span></span>
2. <span data-ttu-id="23168-106">左側のウィンドウで、**[保護]、[DKIM]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="23168-106">In the left pane, select **protection > dkim**.</span></span>
3. <span data-ttu-id="23168-107">ドメインを選択してから、**[このドメインのメッセージに DKIM 署名を追加します]** で **[有効]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="23168-107">Select the domain, and then under **Sign messages for this domain with DKIM signatures**, click **Enable**.</span></span> <span data-ttu-id="23168-108">各ドメインにこの手順を繰り返します。</span><span class="sxs-lookup"><span data-stu-id="23168-108">Repeat this step for each domain.</span></span>

