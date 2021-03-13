---
title: トランスポート ルールを修正する
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751415"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="40095-102">トランスポート ルールを修正する</span><span class="sxs-lookup"><span data-stu-id="40095-102">Fix transport rules</span></span>

<span data-ttu-id="40095-103">カスタムのメール フロー ルールがこのメッセージに影響を与えました。</span><span class="sxs-lookup"><span data-stu-id="40095-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="40095-104">正確なルールを確認するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="40095-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="40095-105">送信結果の **[追加情報]** で、**GUID** または **ポリシー名** を確認します。</span><span class="sxs-lookup"><span data-stu-id="40095-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="40095-106">Exchange 管理シェルを起動します。</span><span class="sxs-lookup"><span data-stu-id="40095-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="40095-107">詳細については、「[Exchange 管理シェルを開く](https://go.microsoft.com/fwlink/?linkid=2101432)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="40095-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="40095-108">(送信時の GUID を使用して) 次のコマンドを実行します: **Get-TransportRule -identity "GUID" | fl \* Description**\*</span><span class="sxs-lookup"><span data-stu-id="40095-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="40095-109">説明を確認して、メッセージに影響を与えた構成済みの条件を確認します。</span><span class="sxs-lookup"><span data-stu-id="40095-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="40095-110">詳細については、「[Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="40095-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
