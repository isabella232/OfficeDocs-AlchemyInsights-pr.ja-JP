---
title: Office 365 Advanced Threat Protection (ATP) に関する問題のトラブルシューティング
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dbdfe2ddcc4afd4477f66ffd060ddb7093af8fd6
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/02/2019
ms.locfileid: "31754860"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="954b3-102">Office 365 ATP の問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="954b3-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="954b3-103">**メール メッセージ配信の遅延通知する**?</span><span class="sxs-lookup"><span data-stu-id="954b3-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="954b3-104">ATP の安全な添付ファイル ポリシーに動的配信オプションを使用してみてください。</span><span class="sxs-lookup"><span data-stu-id="954b3-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="954b3-105">これにより、受信者を悪意のあるファイルから保護しながら、メール メッセージの配信遅延を回避できます。</span><span class="sxs-lookup"><span data-stu-id="954b3-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="954b3-106">**誤検知を報告しますか**?</span><span class="sxs-lookup"><span data-stu-id="954b3-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="954b3-107">分析用にファイルを送信するには、このリンクを使用してください: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="954b3-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="954b3-108">**組織内のユーザーの間で送信されるメールに対して ATP 安全なリンクの保護を有効にできることをご存知ですか**?</span><span class="sxs-lookup"><span data-stu-id="954b3-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="954b3-109">次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="954b3-109">Follow these steps:</span></span>
    1. <span data-ttu-id="954b3-110">https://protection.office.comに移動して、サインインします。</span><span class="sxs-lookup"><span data-stu-id="954b3-110">Go to https://protection.office.com and sign in.</span></span>
    2. <span data-ttu-id="954b3-111">**脅威管理** > **ポリシー** > **安全なリンク**に移動します。</span><span class="sxs-lookup"><span data-stu-id="954b3-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="954b3-112">**[特定の受信者に適用されるポリシー]** で、ポリシーを編集 (または追加) します。</span><span class="sxs-lookup"><span data-stu-id="954b3-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="954b3-113">**組織内で送信されたメッセージに安全なリンクを適用する**を選択します。</span><span class="sxs-lookup"><span data-stu-id="954b3-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="954b3-114">ポリシーを保存し、変更がデータセンターに反映されるまで約 30 分かかります。</span><span class="sxs-lookup"><span data-stu-id="954b3-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="954b3-115">ATP の詳細については、「[Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="954b3-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span></span>