---
title: Office アプリの更新を適用する
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
- "1747"
- "9000140"
ms.openlocfilehash: b5952feaac7ac51faed2a3399c68a87a4227b165
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440583"
---
# <a name="apply-updates-for-office-apps"></a><span data-ttu-id="bb149-102">Office アプリの更新を適用する</span><span class="sxs-lookup"><span data-stu-id="bb149-102">Apply updates for Office apps</span></span>

<span data-ttu-id="bb149-103">既定では、Officeアプリの更新プログラムは無料で、自動的にダウンロードされ、ユーザーの介入なしにバックグラウンドで適用されます。</span><span class="sxs-lookup"><span data-stu-id="bb149-103">By default, updates for Office Apps are free, downloaded automatically, and applied in the background without any user intervention.</span></span> <span data-ttu-id="bb149-104">更新の適用で問題が発生した場合に手動で更新を実行するには、[「Office更新プログラムをインストールする」](https://support.office.com/article/install-office-updates-2ab296f3-7f03-43a2-8e50-46de917611c5)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="bb149-104">To run updates manually if you are running into issues applying updates, see [Install Office updates](https://support.office.com/article/install-office-updates-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span> <span data-ttu-id="bb149-105">詳細については、[「Office インストール時のトラブルシューティング」](https://support.microsoft.com/office/troubleshoot-installing-office-35ff2def-e0b2-4dac-9784-4cf212c1f6c2?ui=en-us&rs=en-us&ad=us#O365Plans=signinorgid)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="bb149-105">For more information, see [Troubleshoot installing Office](https://support.microsoft.com/office/troubleshoot-installing-office-35ff2def-e0b2-4dac-9784-4cf212c1f6c2?ui=en-us&rs=en-us&ad=us#O365Plans=signinorgid).</span></span>

<span data-ttu-id="bb149-106">ユーザーの Office 更新プログラムを管理するには、次のオプションを検討してください。</span><span class="sxs-lookup"><span data-stu-id="bb149-106">To manage Office updates for your users, consider these options:</span></span>

- <span data-ttu-id="bb149-107">必要な更新頻度に基づいて、組織に合った Office 更新チャネルを選択してください。</span><span class="sxs-lookup"><span data-stu-id="bb149-107">Choose the right Office Update Channel for your organization based on the desired frequency of updates.</span></span> <span data-ttu-id="bb149-108">方法については、[「 Microsoft 365 Apps の更新チャネルの概要」](https://docs.microsoft.com/deployoffice/overview-of-update-channels-for-office-365-proplus)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb149-108">To learn how, see [Overview of update channels for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-of-update-channels-for-office-365-proplus).</span></span>

- <span data-ttu-id="bb149-109">更新をインターネットから自動的に適用するか、オンプレミス共有から適用するかを決定します。</span><span class="sxs-lookup"><span data-stu-id="bb149-109">Decide whether to apply updates automatically from the internet or from an on-premises share.</span></span> <span data-ttu-id="bb149-110">方法については、[「Microsoft 365 Apps の更新を管理する方法を選択する」](https://docs.microsoft.com/deployoffice/choose-how-to-manage-updates-to-office-365-proplus)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb149-110">To learn how, see [Choose how to manage updates to Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/choose-how-to-manage-updates-to-office-365-proplus).</span></span>

- <span data-ttu-id="bb149-111">以下の手順で、Office の更新設定を確認し、更新がエンドユーザーのコンピューターにどう適用されるかを制御します。</span><span class="sxs-lookup"><span data-stu-id="bb149-111">Review Office Update Settings to control how updates are applied to end user machines:</span></span>

    - <span data-ttu-id="bb149-112">[Microsoft 365 Apps の更新プログラム設定を構成します](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)。</span><span class="sxs-lookup"><span data-stu-id="bb149-112">[Configure update settings for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus).</span></span>
    - <span data-ttu-id="bb149-113">[インストール後の Office の更新方法を指定します](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)。</span><span class="sxs-lookup"><span data-stu-id="bb149-113">[Define how Office is updated after it's installed](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element).</span></span>

<span data-ttu-id="bb149-114">Office アプリを複数のユーザーに展開する場合は、Office カスタマイズツールを使用して展開用の構成ファイルを作成し、Office 展開ツールを使用してOffice更新プログラムを構成します。</span><span class="sxs-lookup"><span data-stu-id="bb149-114">When deploying Office apps to multiple users, use the Office Customization tool to build configuration files for deployment, and configure Office updates by using the Office Deployment tool.</span></span> <span data-ttu-id="bb149-115">詳細については、「[Office カスタマイズツール](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)と [Office 展開ツールの概要](https://go.microsoft.com/fwlink/p/?LinkID=626065)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb149-115">For more info, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run) and the [Office Deployment tool](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

- <span data-ttu-id="bb149-116">ユーザーグループをセットアップして Office 更新プログラムを展開する方法の例については、「[ローカル ソースから Microsoft 365 Apps を展開する](https://docs.microsoft.com/deployoffice/deploy-office-365-proplus-from-a-local-source)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb149-116">For an example of how to setup user groups to deploy Office updates, see [Deploy Microsoft 365 Apps from a local source](https://docs.microsoft.com/deployoffice/deploy-office-365-proplus-from-a-local-source).</span></span>
-   <span data-ttu-id="bb149-117">Office アプリが開いているために一部のユーザーに Office 更新プログラムが適用されない場合は、ForceAppShutdown 設定の使用を検討してください。</span><span class="sxs-lookup"><span data-stu-id="bb149-117">Consider using the ForceAppShutdown setting in case Office updates are not getting applied to a few users because of open Office apps.</span></span> <span data-ttu-id="bb149-118">詳細については、[FORCEAPPSHUTDOWN プロパティ（プロパティ要素の一部）](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#forceappshutdown-property-part-of-property-element)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb149-118">For more info, see the [FORCEAPPSHUTDOWN property (part of Property element)](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#forceappshutdown-property-part-of-property-element).</span></span> 

<span data-ttu-id="bb149-119">**関連項目**</span><span class="sxs-lookup"><span data-stu-id="bb149-119">**See also**</span></span>

<span data-ttu-id="bb149-120">[Microsoft 365 Apps の更新プロセスの概要](https://docs.microsoft.com/deployoffice/overview-of-the-update-process-for-office-365-proplus)。</span><span class="sxs-lookup"><span data-stu-id="bb149-120">[Overview of the update process for Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-of-the-update-process-for-office-365-proplus).</span></span>  
<span data-ttu-id="bb149-121">[Microsoft 365 Apps の更新プログラムに関するリリース情報](https://docs.microsoft.com/officeupdates/release-notes-office365-proplus)。</span><span class="sxs-lookup"><span data-stu-id="bb149-121">[Release information for updates to Microsoft 365 Apps](https://docs.microsoft.com/officeupdates/release-notes-office365-proplus).</span></span>  
<span data-ttu-id="bb149-122">[Microsoft Endpoint Configuration Manager を使用して Microsoft 365 Apps の更新プログラムを管理する](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager)。</span><span class="sxs-lookup"><span data-stu-id="bb149-122">[Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager).</span></span>  
