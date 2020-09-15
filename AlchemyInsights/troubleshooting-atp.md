---
title: Office 365 Advanced Threat Protection のトラブルシューティング
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 5a13653ba08d8c6b822354ff70f6d276d31cd816
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658919"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="13f5b-102">Office 365 Advanced Threat Protection のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="13f5b-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="13f5b-103">メッセージの配信に遅延がある場合</span><span class="sxs-lookup"><span data-stu-id="13f5b-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="13f5b-104">ATP の安全な添付ファイル ポリシーの [[動的配信]](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) オプションを使用します。</span><span class="sxs-lookup"><span data-stu-id="13f5b-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="13f5b-105">これにより、メッセージの遅延を回避すると同時に、悪意のあるファイルから受信者を保護できるようになります。</span><span class="sxs-lookup"><span data-stu-id="13f5b-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="13f5b-106">Microsoft に誤検知を報告する場合</span><span class="sxs-lookup"><span data-stu-id="13f5b-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="13f5b-107">この[リンク](https://www.microsoft.com/wdsi/filesubmission/)を使用して、分析用にファイルを送信してください。</span><span class="sxs-lookup"><span data-stu-id="13f5b-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="13f5b-108">組織内の受信者間で送信される内部電子メールに安全なリンクの保護機能を有効にする方法</span><span class="sxs-lookup"><span data-stu-id="13f5b-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="13f5b-109">次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="13f5b-109">Follow these steps:</span></span>

  1. <span data-ttu-id="13f5b-110">[https://protection.office.com](https://protection.office.com) に移動して、全体管理者またはセキュリティ管理者のアカウントでサインインします。</span><span class="sxs-lookup"><span data-stu-id="13f5b-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="13f5b-111">左側のナビゲーション ウィンドウにある **[脅威の管理]** で、**[ポリシー]** \> **[安全なリンク]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="13f5b-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="13f5b-112">**[組織全体に適用されるポリシー]** セクションで、ポリシーを選択して **[編集]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="13f5b-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="13f5b-113">**[設定]** の下側にある **[組織内で送信されるメッセージに安全なリンクを適用する]** を有効にします。</span><span class="sxs-lookup"><span data-stu-id="13f5b-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
