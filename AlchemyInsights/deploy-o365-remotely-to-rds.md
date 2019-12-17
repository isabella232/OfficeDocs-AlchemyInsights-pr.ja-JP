---
title: RDS、ターミナル サーバー、または VDI での共有使用のための Office 365 ProPlus の展開
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
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/10/2019
ms.locfileid: "39976359"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="6d737-102">RDS、ターミナル サーバー、または VDI での共有使用のための Office 365 ProPlus の展開</span><span class="sxs-lookup"><span data-stu-id="6d737-102">Deploying Office 365 ProPlus for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="6d737-103">リモート デスクトップ サービス (RDS、旧称ターミナル サービス) を使用して Office 365 ProPlus を展開するには:</span><span class="sxs-lookup"><span data-stu-id="6d737-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
- <span data-ttu-id="6d737-104">Microsoft 365 For Business プラン、または Office 365 Enterprise E3 や Enterprise E5 などの Office 365 ProPlus を含む Office 365 プランが必要です。</span><span class="sxs-lookup"><span data-stu-id="6d737-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE] 
   > <span data-ttu-id="6d737-105">Office 365 Business および Office 365 Business Premium プランには、Office 365 ProPlus は含まれません。</span><span class="sxs-lookup"><span data-stu-id="6d737-105">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5. The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
- <span data-ttu-id="6d737-106">[共有コンピューターのライセンス認証](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)を有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="6d737-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

> [!NOTE]
> <span data-ttu-id="6d737-107">Office 365 ProPlus を共有コンピューターのライセンス認証モードでインストールするには、[Microsoft サポート/回復アシスタント](https://aka.ms/SaRA_OfficeSCA_M365Portal)をダウンロードして実行することもできます。</span><span class="sxs-lookup"><span data-stu-id="6d737-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>

<span data-ttu-id="6d737-108">前提条件の詳細、セットアップ手順、および Office 展開ツールを使用したカスタマイズされたインストールのガイダンスについては、「[リモート デスクトップ サービスを使用して Office 365 ProPlus を展開する](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d737-108">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>

<span data-ttu-id="6d737-109">共有コンピューターのライセンス認証に関連するエラーを修正するには:</span><span class="sxs-lookup"><span data-stu-id="6d737-109">To fix errors related to shared computer activation:</span></span>
- <span data-ttu-id="6d737-110">[Office 365 ProPlus に対する共有コンピューターのライセンス認証に関する問題のトラブルシューティング](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="6d737-110">[Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)</span></span>
- <span data-ttu-id="6d737-111">「[Office 365 ProPlus のライセンス認証の状態をリセットする](https://go.microsoft.com/fwlink/?linkid=2109218)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="6d737-111">See [Reset Office 365 ProPlus activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="6d737-112">Microsoft 365 管理センターから Office 365 ProPlus を RDS にインストールする場合 (***既定のインストール設定を使用***) には、以下の手順を使用します。</span><span class="sxs-lookup"><span data-stu-id="6d737-112">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

1.  <span data-ttu-id="6d737-113">ご利用の Office 365 プランを確認します。</span><span class="sxs-lookup"><span data-stu-id="6d737-113">Check what Office 365 plan you have. Learn how</span></span> <span data-ttu-id="6d737-114">[詳細情報](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d737-114">[Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2.  <span data-ttu-id="6d737-115">必要に応じて別の Office 365 プランに切り替えます。</span><span class="sxs-lookup"><span data-stu-id="6d737-115">If necessary, switch to a different Office 365 plan. Learn how</span></span> <span data-ttu-id="6d737-116">[詳細情報](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d737-116">[Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span></span>
3.  <span data-ttu-id="6d737-117">他の Office 365 プランを使用して Office が RDS サーバーに既にインストールされている場合には、アンインストールします。</span><span class="sxs-lookup"><span data-stu-id="6d737-117">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it. For example, by going to Control Panel  Uninstall a program. Uninstall using Microsoft Support and Recovery Assistant if you're running into issues.</span></span> <span data-ttu-id="6d737-118">たとえば、[**コントロール パネル**] >  [**プログラムのアンインストール**] の順に移動して行います。</span><span class="sxs-lookup"><span data-stu-id="6d737-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="6d737-119">問題が発生した場合には、[Microsoft サポート/回復アシスタント](https://aka.ms/SARA-OfficeUninstall-Alchemy)を使用してアンインストールしてください。</span><span class="sxs-lookup"><span data-stu-id="6d737-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4.  <span data-ttu-id="6d737-120">RDS サーバーで、管理者アカウントを使用して Microsoft 365 管理センターにサインインし、[Office 365 ProPlus をインストール](https://portal.office.com/OLS/MySoftware.aspx)します。</span><span class="sxs-lookup"><span data-stu-id="6d737-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5.  <span data-ttu-id="6d737-121">Office のインストール後は、Office アプリケーションを***開いたり、サインインしたりしないでください***。</span><span class="sxs-lookup"><span data-stu-id="6d737-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6.  <span data-ttu-id="6d737-122">RDS サーバーで、次の手順に従ってレジストリを編集し、共有コンピューターのライセンス認証を有効にします。</span><span class="sxs-lookup"><span data-stu-id="6d737-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="6d737-123">画面の左下隅にある Windows ボタンを右クリックし、[**実行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="6d737-123">Right-click the Windows button in the lower left-hand corner of your screen and select Run. In the Open box, type **regedit**, and then select OK.</span></span> <span data-ttu-id="6d737-124">[名前] ボックスに **regedit** と入力し、[**OK**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="6d737-124">In the Open box, type outlook.exe /importnk2, and then select OK.</span></span>
   2. <span data-ttu-id="6d737-125">レジストリ エディターがデバイスに変更を加えられるようにするかどうかを尋ねるプロンプトが表示されたら、[**はい**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="6d737-125">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="6d737-126">レジストリ エディターで、HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration に文字列値 **SharedComputerLicensing** を追加し、1 を設定します。</span><span class="sxs-lookup"><span data-stu-id="6d737-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="6d737-127">RDS サーバーで***エンド ユーザーとしてサインインし***、[共有コンピューターのライセンス認証が Office 365 ProPlus に対して有効になっていることを確認します](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)。</span><span class="sxs-lookup"><span data-stu-id="6d737-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

