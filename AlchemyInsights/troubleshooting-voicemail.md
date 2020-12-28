---
title: 'ボイスメールのトラブルシューティング '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/09/2020
ms.locfileid: "49680475"
---
# <a name="troubleshooting-voicemail"></a><span data-ttu-id="3aec3-102">ボイスメールのトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="3aec3-102">Troubleshooting Voicemail</span></span>

<span data-ttu-id="3aec3-103">Busy on Busy 機能が意図的なものであることを確認します。</span><span class="sxs-lookup"><span data-stu-id="3aec3-103">Ensure that the Busy on Busy feature is intentional.</span></span>

<span data-ttu-id="3aec3-104">ユーザーがこの機能を必要としない場合は、以下の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="3aec3-104">If this feature is not needed on this user:</span></span>

1. <span data-ttu-id="3aec3-105">[Teams 管理センター](https://admin.teams.microsoft.com/policies/calling)に移動します。</span><span class="sxs-lookup"><span data-stu-id="3aec3-105">Go to [Teams Admin center](https://admin.teams.microsoft.com/policies/calling).</span></span>
1. <span data-ttu-id="3aec3-106">左のレールの **[通話ポリシー]** で **[音声]** > **[通話ポリシー]** > **[ポリシーの管理]** に移動します。</span><span class="sxs-lookup"><span data-stu-id="3aec3-106">On the left rail navigate **Voice** > **Calling policies** > **Manage Policies** on the **Calling Policy**.</span></span>
1. <span data-ttu-id="3aec3-107">**[ユーザーを管理する]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="3aec3-107">Select **Manage Users**.</span></span>
1. <span data-ttu-id="3aec3-108">ユーザーを検索し、**通話中に Busy on Busy を利用** できるようになっている通話ポリシーを **オフ** に変更します。</span><span class="sxs-lookup"><span data-stu-id="3aec3-108">Search for user and change the Calling Policy to one that has **Busy on Busy is available when in a call** to **Off**.</span></span>
1. <span data-ttu-id="3aec3-109">**[適用]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="3aec3-109">Click **Apply**.</span></span>
> [!NOTE]
> <span data-ttu-id="3aec3-110">ポリシーの変更を複製するには、最大 24 時間かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="3aec3-110">Changes to policies can take up to 24 hours to replicate.</span></span>

<span data-ttu-id="3aec3-111">この機能の詳細については、「[通話中に Busy on Busy 機能を利用](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="3aec3-111">For more information on this feature refer to: [Busy on Busy is available while in a call](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span></span>
