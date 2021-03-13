---
title: Microsoft Defender for Office 365 の安全な添付ファイル ポリシーの例
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751309"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="78eea-102">Microsoft Defender for Office 365 の安全な添付ファイル ポリシーの例</span><span class="sxs-lookup"><span data-stu-id="78eea-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="78eea-103">これらの設定により、メッセージをすぐに配信し、スキャン後に添付ファイルを再添付する "*遅延なし*" というポリシーが有効になります。</span><span class="sxs-lookup"><span data-stu-id="78eea-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="78eea-104">**名前**: 遅延なし</span><span class="sxs-lookup"><span data-stu-id="78eea-104">**Name**: No delays</span></span>
- <span data-ttu-id="78eea-105">**説明**: メッセージをすぐに配信し、スキャン後に添付ファイルを再添付します。</span><span class="sxs-lookup"><span data-stu-id="78eea-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="78eea-106">**応答**: **[動的配信]** オプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="78eea-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="78eea-107">詳細については、「[安全な添付ファイル ポリシー内の動的配信](https://go.microsoft.com/fwlink/?linkid=2092328)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="78eea-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="78eea-108">**[添付ファイルをリダイレクト]** セクションで、**[リダイレクトを有効にする]** オプションを選択して、悪意のある添付ファイルを調査する Microsoft 365 のグローバル管理者、セキュリティ管理者、またはセキュリティ アナリストのメール アドレスを入力します。</span><span class="sxs-lookup"><span data-stu-id="78eea-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="78eea-109">[**適用先**] セクションで、[**受信者のドメイン**] を選んでから、自分のドメインを選びます。</span><span class="sxs-lookup"><span data-stu-id="78eea-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="78eea-110">[**追加**] を選択し、[**OK**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="78eea-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="78eea-111">完了したら、[**保存**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="78eea-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="78eea-112">詳細については、「[Microsoft Defender for Office 365 のフィッシング詐欺対策ポリシーを構成する](https://go.microsoft.com/fwlink/?linkid=2092213)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="78eea-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
