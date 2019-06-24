---
title: Office 365 Advanced Threat Protection のトラブルシューティング
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: b4358fb55a1145833510c6063b520d822f2d1eaf
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "35085891"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="8e9d2-102">Office 365 Advanced Threat Protection のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="8e9d2-102">Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="8e9d2-103">メッセージの配信に遅延がある場合</span><span class="sxs-lookup"><span data-stu-id="8e9d2-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="8e9d2-104">ATP の安全な添付ファイル ポリシーの [[動的配信]](https://docs.microsoft.com/office365/securitycompliance/dynamic-delivery-and-previewing) オプションを使用します。</span><span class="sxs-lookup"><span data-stu-id="8e9d2-104">Use the [Dynamic Delivery](https://docs.microsoft.com/office365/securitycompliance/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="8e9d2-105">これにより、メッセージの遅延を回避すると同時に、悪意のあるファイルから受信者を保護できるようになります。</span><span class="sxs-lookup"><span data-stu-id="8e9d2-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="8e9d2-106">Microsoft に誤検知を報告する場合</span><span class="sxs-lookup"><span data-stu-id="8e9d2-106">Do you want to report false positives or false negatives?</span></span> <span data-ttu-id="8e9d2-107">この[リンク](https://www.microsoft.com/wdsi/filesubmission/)を使用して、分析用にファイルを送信してください。</span><span class="sxs-lookup"><span data-stu-id="8e9d2-107">Use this link to submit your file for analysis:   </span></span>

- <span data-ttu-id="8e9d2-108">組織内の受信者間で送信される内部電子メールに安全なリンクの保護機能を有効にする方法</span><span class="sxs-lookup"><span data-stu-id="8e9d2-108">Did you know that you can enable ATP Safe Links protection for email sent between people in your organization?</span></span> <span data-ttu-id="8e9d2-109">次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="8e9d2-109">Follow these steps:</span></span>

  1. <span data-ttu-id="8e9d2-110">[https://protection.office.com](https://protection.office.com) に移動して、全体管理者またはセキュリティ管理者のアカウントでサインインします。</span><span class="sxs-lookup"><span data-stu-id="8e9d2-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="8e9d2-111">左側のナビゲーション ウィンドウにある **[脅威の管理]** で、**[ポリシー]** \> **[安全なリンク]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8e9d2-111">In the left navigation, under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="8e9d2-112">**[組織全体に適用されるポリシー]** セクションで、ポリシーを選択して **[編集]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="8e9d2-112">In the Policies that apply to the entire organization section, select Default, and then choose Edit (the Edit button resembles a pencil).</span></span>

  4. <span data-ttu-id="8e9d2-113">**[設定]** の下側にある **[組織内で送信されるメッセージに安全なリンクを適用する]** を有効にします。</span><span class="sxs-lookup"><span data-stu-id="8e9d2-113">Select Apply safe links to messages sent within the organization.</span></span>
