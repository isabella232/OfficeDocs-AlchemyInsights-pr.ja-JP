---
title: Office 365 ProPlus を展開して RDS、Terminal Server、または VDI で共有する
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/10/2019
ms.locfileid: "39976359"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="a9413-102">Office 365 ProPlus を展開して RDS、Terminal Server、または VDI で共有する</span><span class="sxs-lookup"><span data-stu-id="a9413-102">Deploying Office 365 ProPlus for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="a9413-103">リモートデスクトップサービス (RDS) を使用して Office 365 ProPlus を展開するには、以前の名前付きターミナルサービスを使用します。</span><span class="sxs-lookup"><span data-stu-id="a9413-103">To deploy Office 365 ProPlus using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
- <span data-ttu-id="a9413-104">Office 365 ProPlus (365 Office Enterprise E3、Enterprise E5 など) を含む、Microsoft 365 For Business プランまたは Office 365 プランを所有している必要があります。</span><span class="sxs-lookup"><span data-stu-id="a9413-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE] 
   > <span data-ttu-id="a9413-105">Office 365 Business および Office 365 Business Premium プランには、Office 365 ProPlus は含まれていません。</span><span class="sxs-lookup"><span data-stu-id="a9413-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
- <span data-ttu-id="a9413-106">[共有コンピューターのライセンス認証](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)を有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="a9413-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

> [!NOTE]
> <span data-ttu-id="a9413-107">Office 365 ProPlus を共有コンピューターのライセンス認証モードでインストールするには、[Microsoft サポート/回復アシスタント](https://aka.ms/SaRA_OfficeSCA_M365Portal)をダウンロードして実行することもできます。</span><span class="sxs-lookup"><span data-stu-id="a9413-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>

<span data-ttu-id="a9413-108">Office 展開ツールを使用してカスタマイズされたインストールの前提条件、セットアップ手順、およびガイダンスの詳細については、「 [Deploy office 365 ProPlus by Using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a9413-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>

<span data-ttu-id="a9413-109">共有コンピューターのライセンス認証に関連するエラーを修正するには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="a9413-109">To fix errors related to shared computer activation:</span></span>
- <span data-ttu-id="a9413-110">「 [Office 365 ProPlus の共有コンピューターのライセンス認証に関する問題のトラブルシューティング](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a9413-110">See [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
- <span data-ttu-id="a9413-111">「 [Reset Office 365 ProPlus activation state](https://go.microsoft.com/fwlink/?linkid=2109218)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a9413-111">See [Reset Office 365 ProPlus activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="a9413-112">***既定のインストール設定を使用***する Microsoft 365 管理センターから RDS に Office 365 ProPlus をインストールする場合は、次の手順を使用します。</span><span class="sxs-lookup"><span data-stu-id="a9413-112">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1.  <span data-ttu-id="a9413-113">どの Office 365 プランを使用しているかを確認します。</span><span class="sxs-lookup"><span data-stu-id="a9413-113">Check what Office 365 plan you have.</span></span> <span data-ttu-id="a9413-114">[詳細情報](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a9413-114">[Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2.  <span data-ttu-id="a9413-115">必要に応じて、別の Office 365 プランに切り替えます。</span><span class="sxs-lookup"><span data-stu-id="a9413-115">If necessary, switch to a different Office 365 plan.</span></span> <span data-ttu-id="a9413-116">[詳細情報](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a9413-116">[Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span></span>
3.  <span data-ttu-id="a9413-117">Office が他の Office 365 プランを使用して RDS サーバーに既にインストールされている場合は、それをアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="a9413-117">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="a9413-118">たとえば、[**コントロールパネル]** > を使用して**プログラムをアンインストール**します。</span><span class="sxs-lookup"><span data-stu-id="a9413-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="a9413-119">問題が発生している場合は[、Microsoft サポート/回復アシスタント](https://aka.ms/SARA-OfficeUninstall-Alchemy)を使用してアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="a9413-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4.  <span data-ttu-id="a9413-120">RDS サーバーで、管理者アカウントを使用して Microsoft 365 管理センターにサインインし、[Office 365 ProPlus をインストール](https://portal.office.com/OLS/MySoftware.aspx)します。</span><span class="sxs-lookup"><span data-stu-id="a9413-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5.  <span data-ttu-id="a9413-121">Office のインストール後は、Office アプリケーションを***開いたり、サインインしたりしないでください***。</span><span class="sxs-lookup"><span data-stu-id="a9413-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6.  <span data-ttu-id="a9413-122">RDS サーバーで、次の手順に従ってレジストリを編集し、共有コンピューターのライセンス認証を有効にします。</span><span class="sxs-lookup"><span data-stu-id="a9413-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="a9413-123">画面の左下隅にある [Windows] ボタンを右クリックし、[**実行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a9413-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="a9413-124">[名前] ボックスに「 **regedit**」と入力し、[ **OK**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a9413-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="a9413-125">レジストリエディターにデバイスの変更を許可するかどうかを確認するメッセージが表示されたら、[**はい**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a9413-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="a9413-126">レジストリ エディターで、HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration に文字列値 **SharedComputerLicensing** を追加し、1 を設定します。</span><span class="sxs-lookup"><span data-stu-id="a9413-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="a9413-127">RDS サーバーで***エンド ユーザーとしてサインインし***、[共有コンピューターのライセンス認証が Office 365 ProPlus に対して有効になっていることを確認します](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)。</span><span class="sxs-lookup"><span data-stu-id="a9413-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

