---
title: Office アプリの更新プログラム チャネルを変更する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 3e1042a38d2289b9ef2396e8300d32f20ddaa703
ms.sourcegitcommit: b5e5f560bf6ef92b4475bd3d91b7df38b5a4b036
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/14/2020
ms.locfileid: "46739832"
---
# <a name="change-update-channels-for-office-apps"></a><span data-ttu-id="2024f-102">Office アプリの更新プログラム チャネルを変更する</span><span class="sxs-lookup"><span data-stu-id="2024f-102">Change update channels for Office apps</span></span>

<span data-ttu-id="2024f-103">新しい Office をインストールする場合は、Office ソフトウェアのダウンロード設定を使用して目的の更新プログラム チャネルを選び、Office アプリをインストール (または再インストール) します。</span><span class="sxs-lookup"><span data-stu-id="2024f-103">For new Office installations, use Office Software Download Settings to select the desired update channel, and then install (or re-install) Office apps.</span></span> <span data-ttu-id="2024f-104">詳細については、[「Office 365 のソフトウェア ダウンロードの設定を管理する」](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365) をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="2024f-104">For more info, see [Manage software download settings in Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365).</span></span> 

<span data-ttu-id="2024f-105">**注** Office のソフトウェア ダウンロードの設定を使用して選択された更新プログラム チャネルは、O365 ポータルを使用して新しいインストールを実行しているすべてのユーザーに適用されます。</span><span class="sxs-lookup"><span data-stu-id="2024f-105">**Note** The update channel selected using the Office Software Download Settings applies to all users performing new installations using the O365 portal.</span></span> <span data-ttu-id="2024f-106">詳細については、[「Microsoft 365 または Office 2019 を PC または Mac にダウンロードしてインストールまたは再インストールする」](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2024f-106">For more info, see [Download and install or reinstall Microsoft 365 or Office 2019 on a PC or Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).</span></span>   

<span data-ttu-id="2024f-107">既存の Office インストールの場合、Office 展開ツール (ODT) を使用して別の更新プログラム チャネルに切り替えます:</span><span class="sxs-lookup"><span data-stu-id="2024f-107">For existing Office installations, use the Office Deployment Tool (ODT) to switch to a different update channel:</span></span>  

1. <span data-ttu-id="2024f-108">[Microsoft ダウンロード センター](https://go.microsoft.com/fwlink/p/?LinkID=626065) から最新バージョンの Office 展開ツール (setup.exe) をダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="2024f-108">Download the latest version of the Office Deployment Tool (setup.exe) from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
2. <span data-ttu-id="2024f-109">切り替えるチャネルの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="2024f-109">Identify the name of the channel that you want to switch to.</span></span> <span data-ttu-id="2024f-110">詳細については、[「Office 展開ツールの構成オプション」](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2024f-110">For more info, see [Configuration options for the Office Deployment Tool](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).</span></span>
3. <span data-ttu-id="2024f-111">適切なチャネル名 (たとえば、update.xml) を指定する構成 XML ファイルを作成します。</span><span class="sxs-lookup"><span data-stu-id="2024f-111">Create a configuration XML file specifying the appropriate channel name, for example, update.xml.</span></span>  

`<Configuration>`<br>
`<Updates Channel="Monthly"/>`<br>
`</Configuration>`<br>

4. <span data-ttu-id="2024f-112">管理者特権のコマンド プロンプトから、setup.exe が置かれているフォルダーに切り替え、次のコマンドを実行します:</span><span class="sxs-lookup"><span data-stu-id="2024f-112">From an elevated command prompt, switch to the folder location where setup.exe resides and run the following command:</span></span>  
    <span data-ttu-id="2024f-113">a. </span><span class="sxs-lookup"><span data-stu-id="2024f-113">a.</span></span> <span data-ttu-id="2024f-114">setup.exe /configure update.xml</span><span class="sxs-lookup"><span data-stu-id="2024f-114">setup.exe /configure update.xml</span></span>
5. <span data-ttu-id="2024f-115">Office アプリケーション (Excel など) を起動し、**[ファイル]** > **[アカウント]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="2024f-115">Start an Office application (such as Excel), and then select **File** > **Account**.</span></span> <span data-ttu-id="2024f-116">[製品情報] セクションで、**[更新オプション]** > **[今すぐ更新]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="2024f-116">In the Product Information section, select **Update Options** > **Update Now**.</span></span>

<span data-ttu-id="2024f-117">詳細については、[「既存の Office アプリの更新プログラム チャネルを切り替える方法」](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2024f-117">For more information, see [How to switch update channels for existing Office Apps](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel).</span></span> 

<span data-ttu-id="2024f-118">選択したユーザーのグループまたは構成マネージャー (SCCM) を使用して更新プログラム チャネルを切り替えるには、GPO を使用して更新プログラム チャネルの設定を構成します。</span><span class="sxs-lookup"><span data-stu-id="2024f-118">For switching update channels for a selected group of users or by using Configuration Manager (SCCM), configure the Update Channel setting using GPO.</span></span> <span data-ttu-id="2024f-119">詳細については、[「Microsoft 365 アプリの更新プログラム チャネルの概要」](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2024f-119">For more info, see [Overview of update channels for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy).</span></span> <span data-ttu-id="2024f-120">詳細については、[「IT 担当者向け Office 365 ProPlus チャネルを管理する方法」](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813)、[「Microsoft Endpoint Configuration Manager を使用して Microsoft 365 アプリの更新を管理する」](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2024f-120">For details, see [How to manage Office 365 ProPlus Channels for IT Pros](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) and [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).</span></span>