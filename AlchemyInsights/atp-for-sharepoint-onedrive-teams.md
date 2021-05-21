---
title: SharePoint、OneDrive、Microsoft Teams 用の Microsoft Defender for Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 7d2ed7bc4c7d99cd01dadc12e38762903d6d8ab3
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543582"
---
# <a name="microsoft-defender-for-office-365-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="b59c1-102">SharePoint、OneDrive、Microsoft Teams 用の Microsoft Defender for Office 365</span><span class="sxs-lookup"><span data-stu-id="b59c1-102">Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="b59c1-103">次の手順に従って、Microsoft Defender for Office 365 を有効にします。</span><span class="sxs-lookup"><span data-stu-id="b59c1-103">Follow these steps to enable Microsoft Defender for Office 365:</span></span>

1. <span data-ttu-id="b59c1-104">[https://protection.office.com](https://protection.office.com) に移動して、全体管理者またはセキュリティ管理者のアカウントでサインインします。</span><span class="sxs-lookup"><span data-stu-id="b59c1-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="b59c1-105">左側のナビゲーション ウィンドウにある **[脅威の管理]** で、**[ポリシー]** \> **[安全な添付ファイル]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="b59c1-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="b59c1-106">**[SharePoint、OneDrive、Microsoft Teams 用の Defender for Office 365 を有効にする]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="b59c1-106">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="b59c1-107">[アクティビティ アラート ポリシーを作成](/microsoft-365/compliance/create-activity-alerts)して、悪意のあるファイルが検出されたときに通知を受け取るようにします。</span><span class="sxs-lookup"><span data-stu-id="b59c1-107">[Create an activity alert policy](/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="b59c1-108">詳細な手順については、「[SharePoint、OneDrive、Microsoft Teams に対して安全な添付ファイルをオンにする](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b59c1-108">For complete instructions, see this [Turn on Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="b59c1-109">**注**: Microsoft Defender for Office 365 は、SharePoint Online、OneDrive for Business、または Microsoft Teams のファイルを 1 つずつスキャンしないようになっています。</span><span class="sxs-lookup"><span data-stu-id="b59c1-109">**Note**: By design, Microsoft Defender for Office 365 doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="b59c1-110">ファイルは、共有のアクティビティ、ゲストのアクティビティ、および脅威のシグナルを使用して悪意のあるファイルを特定するプロセスによって、非同期的にスキャンされます。</span><span class="sxs-lookup"><span data-stu-id="b59c1-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="b59c1-111">詳細については、「[SharePoint、OneDrive、Microsoft Teams の安全な添付ファイル](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b59c1-111">For more information, see [Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
