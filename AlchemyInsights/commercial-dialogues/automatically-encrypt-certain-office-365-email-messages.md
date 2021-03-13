---
title: 特定の Office 365 メール メッセージを自動的に暗号化
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751328"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="7dcca-102">特定の Office 365 メール メッセージを自動的に暗号化</span><span class="sxs-lookup"><span data-stu-id="7dcca-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="7dcca-103">ユーザーが特定の外部ユーザーや組織に送信するメッセージを自動的に暗号化することができます。</span><span class="sxs-lookup"><span data-stu-id="7dcca-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="7dcca-104">これを実現するには、以下の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="7dcca-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="7dcca-105">[Exchange 管理センター](https://outlook.office365.com/ecp/) で、**[メール フロー]、[ルール]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="7dcca-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="7dcca-106">**[}新規 (+)]** アイコンをクリックし、**[メッセージに Office 365 Message Encryption と権利保護を適用する]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="7dcca-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="7dcca-107">**[名前]** には、*DrToniRamos@gmail.com に送信されるメッセージを暗号化* など、ルールの名前を入力します。</span><span class="sxs-lookup"><span data-stu-id="7dcca-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="7dcca-108">**[このルールを適用]** で、**[受信者]、[この人物である]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="7dcca-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="7dcca-109">**[メンバーの選択]** ウィンドウで、暗号化ルールを適用するユーザーの名前を選択し、**[追加]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="7dcca-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="7dcca-110">ユーザーの追加が完了したら、[**OK**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="7dcca-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="7dcca-111">**[次を実行]** フィールドの横にある **[いずれかを選択]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="7dcca-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="7dcca-112">**[RMS テンプレート]** のドロップダウン メニューで **[暗号化]** を選択し、**[OK]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="7dcca-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="7dcca-113">(このオプションが表示されない場合は、ご利用のプランに自動暗号化が含まれていないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="7dcca-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="7dcca-114">ただし、追加することができます。)</span><span class="sxs-lookup"><span data-stu-id="7dcca-114">But you can add it!)</span></span>
9. <span data-ttu-id="7dcca-115">省略可能な選択を選びます (この時点でできる省略可能な選択の一覧のうち、多くは簡単にするために既定の設定のままにしておくことができます)。</span><span class="sxs-lookup"><span data-stu-id="7dcca-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="7dcca-116">**[保存]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="7dcca-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="7dcca-117">いつでも戻ってこのルールを編集することができます。</span><span class="sxs-lookup"><span data-stu-id="7dcca-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="7dcca-118">OME のメール フロー ルールの作成の手順については、「[Office 365 でメール メッセージを暗号化するためにメール フロー ルールを定義する](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7dcca-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

