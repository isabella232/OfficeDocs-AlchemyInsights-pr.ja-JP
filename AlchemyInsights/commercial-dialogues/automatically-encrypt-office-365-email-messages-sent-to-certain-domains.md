---
title: 特定のドメインに送信されたOffice 365のメールメッセージを自動的に暗号化
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751317"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="97984-102">特定のドメインに送信されたOffice 365のメールメッセージを自動的に暗号化</span><span class="sxs-lookup"><span data-stu-id="97984-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="97984-103">[Exchange 管理センター](https://outlook.office365.com/ecp/) で、**[メール フロー]、[ルール]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="97984-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="97984-104">**[}新規 (+)]** アイコンをクリックし、**[メッセージに Office 365 Message Encryption と権利保護を適用する]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="97984-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="97984-105">**[名前]** には、*contoso.com に送信されるメッセージを暗号化* など、ルールの名前を入力します。</span><span class="sxs-lookup"><span data-stu-id="97984-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="97984-106">**[このルールを適用]** で、**[受信者]、[ドメインが次の値である]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="97984-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="97984-107">**contoso.com** などのドメイン名を入力します。</span><span class="sxs-lookup"><span data-stu-id="97984-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="97984-108">**追加 (+)** アイコンをクリックし、**[OK]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="97984-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="97984-109">**[次を実行]** フィールドの横にある **[いずれかを選択]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="97984-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="97984-110">**[RMS テンプレート]** のドロップダウン メニューで **[暗号化]** を選択し、**[OK]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="97984-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="97984-111">(このオプションが表示されない場合は、ご利用のプランに自動暗号化が含まれていないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="97984-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="97984-112">ただし、追加することができます。)</span><span class="sxs-lookup"><span data-stu-id="97984-112">But you can add it!)</span></span>
9. <span data-ttu-id="97984-113">省略可能な選択を選びます (この時点でできる省略可能な選択の一覧のうち、多くは簡単にするために既定の設定のままにしておくことができます)。</span><span class="sxs-lookup"><span data-stu-id="97984-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="97984-114">**[保存]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="97984-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="97984-115">いつでも戻ってこのルールを編集することができます。</span><span class="sxs-lookup"><span data-stu-id="97984-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="97984-116">暗号化のルール作成の詳細については、「[Office 365 でメール メッセージを暗号化するためにメール フロー ルールを定義する](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="97984-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>