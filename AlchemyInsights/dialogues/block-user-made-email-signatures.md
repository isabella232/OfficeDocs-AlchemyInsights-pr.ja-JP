---
title: ユーザーが作成した電子メールの署名をブロックする
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243799"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="d7aa5-102">ユーザーが作成した電子メールの署名をブロックする</span><span class="sxs-lookup"><span data-stu-id="d7aa5-102">Block user-made email signatures</span></span>

<span data-ttu-id="d7aa5-103">次の解決策は、Outlook on the Web で作成された電子メール署名にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="d7aa5-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="d7aa5-104">オンプレミスの Exchange Serverが ある場合にのみ、Outlook アプリで署名をブロックできます。</span><span class="sxs-lookup"><span data-stu-id="d7aa5-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="d7aa5-105">管理センターで、**[管理センター]** > **[Exchange]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="d7aa5-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="d7aa5-106">**[アクセス許可]** > **[Outlook Web App ポリシー]** の順にクリックします。</span><span class="sxs-lookup"><span data-stu-id="d7aa5-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="d7aa5-107">ポリシーを選択し、鉛筆アイコンをクリックして編集します。</span><span class="sxs-lookup"><span data-stu-id="d7aa5-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="d7aa5-108">**[機能]** > **[その他のオプション]** の順にクリックします。</span><span class="sxs-lookup"><span data-stu-id="d7aa5-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="d7aa5-109">**[ユーザー エクスペリエンス]** で、**[電子メールの署名]** チェックボックスをオフにし、**[保存]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="d7aa5-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="d7aa5-110">**重要:** このチェックボックスをオフにする前に署名が追加された場合でも、ユーザーはその署名を使用できます。</span><span class="sxs-lookup"><span data-stu-id="d7aa5-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="d7aa5-111">それらを削除するように依頼してください。</span><span class="sxs-lookup"><span data-stu-id="d7aa5-111">Ask them to remove it.</span></span>
