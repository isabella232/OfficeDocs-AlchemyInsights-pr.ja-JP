---
title: Microsoft Defender for Office 365 (ATP) の問題のトラブルシューティング
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
ms.openlocfilehash: cf54d5b3b854587202ff1b575889b9602228dd06
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801412"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="da57c-102">Office 365 ATP の問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="da57c-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="da57c-103">**メール メッセージ配信の遅延通知する** ?</span><span class="sxs-lookup"><span data-stu-id="da57c-103">**Notice delays with email message delivery** ?</span></span> <span data-ttu-id="da57c-104">ATP の安全な添付ファイル ポリシーに動的配信オプションを使用してみてください。</span><span class="sxs-lookup"><span data-stu-id="da57c-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="da57c-105">これにより、受信者を悪意のあるファイルから保護しながら、メール メッセージの配信遅延を回避できます。</span><span class="sxs-lookup"><span data-stu-id="da57c-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="da57c-106">**誤検知を報告しますか** ?</span><span class="sxs-lookup"><span data-stu-id="da57c-106">**Do you want to report false positives or false negatives** ?</span></span> <span data-ttu-id="da57c-107">分析用にファイルを送信するには、このリンクを使用してください: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="da57c-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="da57c-108">**組織内のユーザーの間で送信されるメールに対して ATP 安全なリンクの保護を有効にできることをご存知ですか** ?</span><span class="sxs-lookup"><span data-stu-id="da57c-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization** ?</span></span> <span data-ttu-id="da57c-109">次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="da57c-109">Follow these steps:</span></span>
    1. <span data-ttu-id="da57c-110"> https://protection.office.comに移動して、サインインします。</span><span class="sxs-lookup"><span data-stu-id="da57c-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="da57c-111">**脅威管理** > **ポリシー** > **安全なリンク** に移動します。</span><span class="sxs-lookup"><span data-stu-id="da57c-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="da57c-112">**[特定の受信者に適用されるポリシー]** で、ポリシーを編集 (または追加) します。</span><span class="sxs-lookup"><span data-stu-id="da57c-112">Under **Policies that apply to specific recipients** , edit (or add) a policy.</span></span>
    4. <span data-ttu-id="da57c-113">**組織内で送信されたメッセージに安全なリンクを適用する** を選択します。</span><span class="sxs-lookup"><span data-stu-id="da57c-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="da57c-114">ポリシーを保存し、変更がデータセンターに反映されるまで約 30 分かかります。</span><span class="sxs-lookup"><span data-stu-id="da57c-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="da57c-115">ATP の詳細については、「[Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="da57c-115">To get more help with ATP, see [Microsoft Defender for Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>