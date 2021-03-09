---
title: ジャーナル ルールの作成
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004299"
- "7677"
ms.openlocfilehash: b0b95f8b6460418d92314dede2ca8bc1326b033e
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527905"
---
# <a name="create-a-journal-rule"></a><span data-ttu-id="f333e-102">ジャーナル ルールの作成</span><span class="sxs-lookup"><span data-stu-id="f333e-102">Create a journal rule</span></span>

<span data-ttu-id="f333e-103">次の操作を実行してください。</span><span class="sxs-lookup"><span data-stu-id="f333e-103">Here's how:</span></span>

1. <span data-ttu-id="f333e-104">[Exchange 管理センター](https://go.microsoft.com/fwlink/p/?linkid=2059104)で、**[コンプライアンス管理]** > **[ジャーナル ルール]** の順に移動し、**[追加 +]** アイコンを選択します。</span><span class="sxs-lookup"><span data-stu-id="f333e-104">In the [Exchange admin center](https://go.microsoft.com/fwlink/p/?linkid=2059104), go to **compliance management** > **journal rules**, and then select the **Add (+)** icon.</span></span>
2. <span data-ttu-id="f333e-105">**[ジャーナル ルールの新規作成]** でジャーナル ルールの名前を指定し、次のフィールドを入力します。</span><span class="sxs-lookup"><span data-stu-id="f333e-105">In **new journal rule**, provide a name for the journal rule and then compete the following fields:</span></span>  
    - <span data-ttu-id="f333e-106">**ジャーナル レポートの送信先**: すべてのジャーナル レポートを受信するジャーナル メールボックスのアドレスを入力します。</span><span class="sxs-lookup"><span data-stu-id="f333e-106">**Send journal reports to**: Enter the address of the journaling mailbox that will receive all the journal reports.</span></span>  
    - <span data-ttu-id="f333e-107">**メッセージの送信先または受信元が次の場合**: ルールの対象となる受信者を指定します。</span><span class="sxs-lookup"><span data-stu-id="f333e-107">**If the message is sent to or received from**: Specify the recipient that the rule will target.</span></span> <span data-ttu-id="f333e-108">特定の受信者を指定するか、またはすべてのメッセージにルールを適用できます。</span><span class="sxs-lookup"><span data-stu-id="f333e-108">You can either select a specific recipient or apply the rule to all messages.</span></span>  
    - <span data-ttu-id="f333e-109">**以下のメッセージをジャーナリングする**: ジャーナル ルールの範囲を指定します。</span><span class="sxs-lookup"><span data-stu-id="f333e-109">**Journal the following messages**: Specify the scope of the journal rule.</span></span> <span data-ttu-id="f333e-110">内部メッセージのみ、外部メッセージのみ、または発信元や宛先に関係なくすべてのメッセージをジャーナリングできます。</span><span class="sxs-lookup"><span data-stu-id="f333e-110">You can journal only the internal messages, only the external messages, or all messages regardless of origin or destination.</span></span>
3. <span data-ttu-id="f333e-111">**[保存]** を選択して、ジャーナル ルールを作成します。</span><span class="sxs-lookup"><span data-stu-id="f333e-111">Select **Save** to create the journal rule.</span></span>
