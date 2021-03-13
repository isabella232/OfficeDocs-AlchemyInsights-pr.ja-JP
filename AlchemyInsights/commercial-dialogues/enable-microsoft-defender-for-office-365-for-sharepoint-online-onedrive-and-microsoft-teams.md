---
title: SharePoint、OneDrive、Microsoft Teams の Microsoft Defender for Office 365 を有効にする
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
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751197"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="1b781-102">SharePoint、OneDrive、Microsoft Teams の Microsoft Defender for Office 365 を有効にする</span><span class="sxs-lookup"><span data-stu-id="1b781-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive and Microsoft Teams</span></span>

1. <span data-ttu-id="1b781-103">グローバル管理者またはセキュリティ管理者の資格情報を使用して、[Office 365 セキュリティ/コンプライアンス センター](https://protection.office.com/)にログインします。</span><span class="sxs-lookup"><span data-stu-id="1b781-103">Using your global admin or security admin credentials, log in to the [Office 365 Security and Compliance Center](https://protection.office.com/).</span></span>
2. <span data-ttu-id="1b781-104">左側のウィンドウで **[脅威の管理]** を選択し、**[ポリシー]** > [[安全な添付ファイル]](https://protection.office.com/safeattachment) の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="1b781-104">Select **Threat management** in the left pane, and then select **Policy** > [Safe attachments](https://protection.office.com/safeattachment).</span></span>
3. <span data-ttu-id="1b781-105">**[SharePoint、OneDrive、Microsoft Teams 用の Microsoft Defender for Office 365 をオンにする]** を選択してから **[保存]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="1b781-105">Select **Turn on Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then select **Save**.</span></span>
    > [!TIP]
    >
    > - <span data-ttu-id="1b781-106">グローバル管理者または SharePoint Online 管理者として、**DisallowInfectedFileDownload** パラメーターを *true* に設定して、次の PowerShell コマンドレットを実行します: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span><span class="sxs-lookup"><span data-stu-id="1b781-106">As a global admin or a SharePoint Online admin, run the following PowerShell cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span></span>
    > - [<span data-ttu-id="1b781-107">検出されたファイルに対する警告を設定する</span><span class="sxs-lookup"><span data-stu-id="1b781-107">Set up alerts for detected files</span></span>](https://go.microsoft.com/fwlink/?linkid=2092110)

<span data-ttu-id="1b781-108">詳細については、「[SharePoint、OneDrive、Microsoft Teams 用の Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092041)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1b781-108">For more information, see [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span></span>
