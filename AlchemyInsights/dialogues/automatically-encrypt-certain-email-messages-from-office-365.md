---
title: Office 365 で特定の メール メッセージを自動的に暗号化
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527922"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="9c1af-102">Office 365 で特定の メール メッセージを自動的に暗号化</span><span class="sxs-lookup"><span data-stu-id="9c1af-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="9c1af-103">[Exchange 管理センター](https://outlook.office365.com/ecp/) で、**[メール フロー]、[ルール]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="9c1af-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="9c1af-104">**[}新規 (+)]** アイコンをクリックし、**[メッセージに Office 365 Message Encryption と権利保護を適用する]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="9c1af-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="9c1af-105">**[名前]** には、*すべてのメッセージを暗号化* など、ルールの名前を入力します。</span><span class="sxs-lookup"><span data-stu-id="9c1af-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="9c1af-106">**[このルールを適用します]** の **[すべてのメッセージに適用]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="9c1af-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="9c1af-107">**[次を実行]** フィールドの横にある **[いずれかを選択]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="9c1af-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="9c1af-108">**[RMS テンプレート]** のドロップダウン メニューで **[暗号化]** を選択し、**[OK]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="9c1af-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="9c1af-109">(このオプションが表示されない場合は、ご利用のプランに自動暗号化が含まれていないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="9c1af-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="9c1af-110">ただし、追加することができます。)</span><span class="sxs-lookup"><span data-stu-id="9c1af-110">But you can add it!)</span></span>
7. <span data-ttu-id="9c1af-111">**[このルールをセキュリティ レベルで監査]** チェックボックスをオンにして、必要なレベルを選択します。</span><span class="sxs-lookup"><span data-stu-id="9c1af-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="9c1af-112">ご所属の会社で、すべてのメールを暗号化して送信する契約上の義務がある場合は、レベルを **[高]** に設定することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="9c1af-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="9c1af-113">**[このルールのモデルを選択]** で、**[強制]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="9c1af-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="9c1af-114">省略可能な選択を選びます (この時点でできる省略可能な選択の一覧のうち、多くは簡単にするために既定の設定のままにしておくことができます)。</span><span class="sxs-lookup"><span data-stu-id="9c1af-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="9c1af-115">**[保存]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="9c1af-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="9c1af-116">いつでも戻ってこのルールを編集することができます。</span><span class="sxs-lookup"><span data-stu-id="9c1af-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="9c1af-117">暗号化のルール作成の詳細については、「[Office 365 でメール メッセージを暗号化するためにメール フロー ルールを定義する](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9c1af-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

