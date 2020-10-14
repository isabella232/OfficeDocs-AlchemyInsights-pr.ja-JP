---
title: Office 365 Advanced Threat Protection (ATP) に関する問題のトラブルシューティング
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 4164781a331ec919811332e94636449e9d88430d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758070"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="2105f-102">Office 365 ATP の問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="2105f-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="2105f-103">**メール メッセージ配信の遅延通知する**?</span><span class="sxs-lookup"><span data-stu-id="2105f-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="2105f-104">ATP の安全な添付ファイル ポリシーに動的配信オプションを使用してみてください。</span><span class="sxs-lookup"><span data-stu-id="2105f-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="2105f-105">これにより、受信者を悪意のあるファイルから保護しながら、メール メッセージの配信遅延を回避できます。</span><span class="sxs-lookup"><span data-stu-id="2105f-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="2105f-106">**誤検知を報告しますか**?</span><span class="sxs-lookup"><span data-stu-id="2105f-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="2105f-107">分析用にファイルを送信するには、このリンクを使用してください: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="2105f-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="2105f-108">**組織内のユーザーの間で送信されるメールに対して ATP 安全なリンクの保護を有効にできることをご存知ですか**?</span><span class="sxs-lookup"><span data-stu-id="2105f-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="2105f-109">次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="2105f-109">Follow these steps:</span></span>
    1. <span data-ttu-id="2105f-110">https://protection.office.comに移動して、サインインします。</span><span class="sxs-lookup"><span data-stu-id="2105f-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="2105f-111">**脅威管理** > **ポリシー** > **安全なリンク**に移動します。</span><span class="sxs-lookup"><span data-stu-id="2105f-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="2105f-112">**[特定の受信者に適用されるポリシー]** で、ポリシーを編集 (または追加) します。</span><span class="sxs-lookup"><span data-stu-id="2105f-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="2105f-113">**組織内で送信されたメッセージに安全なリンクを適用する**を選択します。</span><span class="sxs-lookup"><span data-stu-id="2105f-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="2105f-114">ポリシーを保存し、変更がデータセンターに反映されるまで約 30 分かかります。</span><span class="sxs-lookup"><span data-stu-id="2105f-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="2105f-115">ATP の詳細については、「[Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2105f-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>