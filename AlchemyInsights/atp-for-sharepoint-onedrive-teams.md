---
title: SharePoint、OneDrive、Microsoft Teams 用の ATP
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: e9437d04815d4ca2f55cf9133ef6a4b429cd2476
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508417"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="81573-102">SharePoint、OneDrive、Microsoft Teams 用の ATP</span><span class="sxs-lookup"><span data-stu-id="81573-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="81573-103">次の手順を実行して、Advanced Threat Protection を有効にします。</span><span class="sxs-lookup"><span data-stu-id="81573-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="81573-104">[https://protection.office.com](https://protection.office.com) に移動して、全体管理者またはセキュリティ管理者のアカウントでサインインします。</span><span class="sxs-lookup"><span data-stu-id="81573-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="81573-105">左側のナビゲーション ウィンドウにある **[脅威の管理]** で、**[ポリシー]** \> **[安全な添付ファイル]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="81573-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="81573-106">**[SharePoint、OneDrive、および Microsoft Teams に対して ATP を有効にする]** をオンにします。</span><span class="sxs-lookup"><span data-stu-id="81573-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="81573-107">[アクティビティ アラート ポリシーを作成](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts)して、悪意のあるファイルが検出されたときに通知を受け取るようにします。</span><span class="sxs-lookup"><span data-stu-id="81573-107">[Create an activity alert policy](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="81573-108">詳細な手順については、この[トピック](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="81573-108">For complete instructions, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="81573-109">**注**: ATP は、SharePoint Online、OneDrive for Business、または Microsoft Teams のファイルを 1 つずつスキャンしないようになっています。</span><span class="sxs-lookup"><span data-stu-id="81573-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="81573-110">ファイルは、共有のアクティビティ、ゲストのアクティビティ、および脅威のシグナルを使用して悪意のあるファイルを特定するプロセスによって、非同期的にスキャンされます。</span><span class="sxs-lookup"><span data-stu-id="81573-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="81573-111">詳細については、この[トピック](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="81573-111">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
