---
title: Officeアプリの自動更新を制御する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440564"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="29dc6-102">Officeアプリの自動更新を制御する</span><span class="sxs-lookup"><span data-stu-id="29dc6-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="29dc6-103">既定では、Office アプリの更新は自動的にダウンロードされ、ユーザーの介入なしにバックグラウンドで適用されます。</span><span class="sxs-lookup"><span data-stu-id="29dc6-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="29dc6-104">ただし、管理者は Office 更新プログラムの設定を使用して、更新の適用方法を制御できます。</span><span class="sxs-lookup"><span data-stu-id="29dc6-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="29dc6-105">更新設定で、管理者は自動更新を有効または無効にしたり、Officeの **[今すぐ更新する]** ボタンを表示または非表示にしたり、更新の期限を設定したりできます。</span><span class="sxs-lookup"><span data-stu-id="29dc6-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="29dc6-106">詳細については、次を参照してください。</span><span class="sxs-lookup"><span data-stu-id="29dc6-106">For detailed information, see:</span></span>

- [<span data-ttu-id="29dc6-107">Office の更新設定を構成する</span><span class="sxs-lookup"><span data-stu-id="29dc6-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="29dc6-108">Office の自動更新が有効になっていません</span><span class="sxs-lookup"><span data-stu-id="29dc6-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="29dc6-109">インストール後の Office の更新方法を指定する</span><span class="sxs-lookup"><span data-stu-id="29dc6-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="29dc6-110">クライアント マシンに適用されている既存の更新設定を確認するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="29dc6-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="29dc6-111">**Start** > **Run** > **Regedit** に移動して、レジストリエディタを開きます。</span><span class="sxs-lookup"><span data-stu-id="29dc6-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="29dc6-112">以下の場所に移動し、Office の更新プログラムの設定を確認します。</span><span class="sxs-lookup"><span data-stu-id="29dc6-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="29dc6-113">a. </span><span class="sxs-lookup"><span data-stu-id="29dc6-113">a.</span></span> <span data-ttu-id="29dc6-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span><span class="sxs-lookup"><span data-stu-id="29dc6-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office</span></span>\  
    <span data-ttu-id="29dc6-115">b. </span><span class="sxs-lookup"><span data-stu-id="29dc6-115">b.</span></span> <span data-ttu-id="29dc6-116">ClickToRun\Configuration</span><span class="sxs-lookup"><span data-stu-id="29dc6-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="29dc6-117">**注** OfficeMgmtCOM キーが設定されている場合、**Office** > **アカウント** > **Office Updates**に「システム管理者によって更新が管理されています」というメッセージが表示される場合があります。</span><span class="sxs-lookup"><span data-stu-id="29dc6-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="29dc6-118">詳細は、「[Microsoft Endpoint Configuration Manager を使用して Microsoft 365 Apps の更新プログラムを管理する](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="29dc6-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  