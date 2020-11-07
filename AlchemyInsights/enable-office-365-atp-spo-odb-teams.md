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
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801054"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="bef35-102">SharePoint、OneDrive、Microsoft Teams の Microsoft Defender for Office 365 を有効にする</span><span class="sxs-lookup"><span data-stu-id="bef35-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="bef35-103"> https://protection.office.com に移動し、サインインします。</span><span class="sxs-lookup"><span data-stu-id="bef35-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="bef35-104">**脅威管理** > **ポリシー** > **安全な添付ファイル** を選択します。</span><span class="sxs-lookup"><span data-stu-id="bef35-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="bef35-105">[ **ATP を SharePoint、OneDrive、Microsoft Teams で有効にする** ]を選択し、[ **保存** ]をクリックします。</span><span class="sxs-lookup"><span data-stu-id="bef35-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams** , and then click **Save**.</span></span>
4. <span data-ttu-id="bef35-106">(推奨) グローバル管理者または SharePoint Online 管理者として、 **DisallowInfectedFileDownload** パラメーターを *true* に設定して [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) コマンドレットを実行します。</span><span class="sxs-lookup"><span data-stu-id="bef35-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="bef35-107">(推奨) 検出されたファイルに対する[警告を設定](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files)します。</span><span class="sxs-lookup"><span data-stu-id="bef35-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="bef35-108">ATP は SharePoint Online、OneDrive、または Microsoft Teams のすべてのファイルをスキャンしません。</span><span class="sxs-lookup"><span data-stu-id="bef35-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="bef35-109">ファイルは、共有イベントおよびゲスト アクティビティ イベントをスマート ヒューリスティックおよび脅威のシグナルと共に使用して悪質なファイルを特定するプロセスを通じて、非同期的にスキャンされます。</span><span class="sxs-lookup"><span data-stu-id="bef35-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="bef35-110">「[SharePoint、OneDrive、Microsoft Teams 用の ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bef35-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>