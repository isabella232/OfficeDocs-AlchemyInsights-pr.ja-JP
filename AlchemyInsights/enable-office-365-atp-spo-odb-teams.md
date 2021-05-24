---
title: SharePoint、OneDrive、Microsoft Teams の Office 365 ATP を有効にする
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
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543933"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="42743-102">SharePoint、OneDrive、Microsoft Teams の Microsoft Defender for Office 365 を有効にする</span><span class="sxs-lookup"><span data-stu-id="42743-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="42743-103"> https://protection.office.com に移動し、サインインします。</span><span class="sxs-lookup"><span data-stu-id="42743-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="42743-104">**脅威管理** > **ポリシー** > **安全な添付ファイル** を選択します。</span><span class="sxs-lookup"><span data-stu-id="42743-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="42743-105">**[SharePoint、OneDrive、Microsoft Teams 用の Microsoft Defender for Office 365 を有効にする]** を選択してから、**[保存]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="42743-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="42743-106">(推奨) グローバル管理者または SharePoint Online 管理者として、**DisallowInfectedFileDownload** パラメーターを *true* に設定して [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) コマンドレットを実行します。</span><span class="sxs-lookup"><span data-stu-id="42743-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="42743-107">(推奨) 検出されたファイルに対する[警告を設定](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files)します。</span><span class="sxs-lookup"><span data-stu-id="42743-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="42743-108">Microsoft Defender for Office 365 は、SharePoint Online、OneDrive、Microsoft Teams にあるすべてのファイルをスキャンするわけではありません。</span><span class="sxs-lookup"><span data-stu-id="42743-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="42743-109">ファイルは、共有イベントおよびゲスト アクティビティ イベントをスマート ヒューリスティックおよび脅威のシグナルと共に使用して悪質なファイルを特定するプロセスを通じて、非同期的にスキャンされます。</span><span class="sxs-lookup"><span data-stu-id="42743-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="42743-110">「[SharePoint、OneDrive、Microsoft Teams 用の Microsoft Defender for Office 365](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="42743-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>