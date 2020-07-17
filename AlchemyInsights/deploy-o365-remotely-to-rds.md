---
title: RDS、ターミナル サーバー、または VDI で共有して使用する Microsoft 365 Apps for enterprise の展開
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: fe051cd1dac899dc9bb19d275c352ec6585b6a93
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507591"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="045e0-102">RDS、ターミナル サーバー、または VDI で共有して使用する Microsoft 365 Apps for enterprise の展開</span><span class="sxs-lookup"><span data-stu-id="045e0-102">Deploying Microsoft 365 Apps for enterprise for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="045e0-103">リモート デスクトップ サービス (RDS、旧称ターミナル サービス) を使用して Microsoft 365 Apps for enterprise を展開するには:</span><span class="sxs-lookup"><span data-stu-id="045e0-103">To deploy Microsoft 365 Apps for enterprise using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
- <span data-ttu-id="045e0-104">Microsoft 365 For Business プラン、あるいは Microsoft 365 Apps for enterprise を含む Office 365 プラン (Office 365 Enterprise E3、Enterprise E5 など) が必要です。</span><span class="sxs-lookup"><span data-stu-id="045e0-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE] 
   > <span data-ttu-id="045e0-105">Microsoft 365 Apps for business と Microsoft 365 Business Premium および Standard プランには Microsoft 365 Apps for enterprise は含まれていません。</span><span class="sxs-lookup"><span data-stu-id="045e0-105">The Microsoft 365 Apps for business and Microsoft 365 Business Premium Standard plans do not include Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="045e0-106">[共有コンピューターのライセンス認証](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)を有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="045e0-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

> [!NOTE]
> <span data-ttu-id="045e0-107">[Microsoft サポート/回復アシスタント](https://aka.ms/SaRA_OfficeSCA_M365Portal)をダウンロードして実行することによっても、Microsoft 365 Apps for enterprise を共有コンピューターのライセンス認証モードでインストールできます。</span><span class="sxs-lookup"><span data-stu-id="045e0-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>

<span data-ttu-id="045e0-108">Office 展開ツールを使用したカスタム インストールの前提条件、セットアップ手順、ガイダンスについて詳しくは、「[リモート デスクトップ サービスを使用して Microsoft 365 Apps for enterprise を展開する](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="045e0-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>

<span data-ttu-id="045e0-109">共有コンピューターのライセンス認証に関連するエラーを修正するには:</span><span class="sxs-lookup"><span data-stu-id="045e0-109">To fix errors related to shared computer activation:</span></span>
- <span data-ttu-id="045e0-110">「[Microsoft 365 Apps for enterprise に対する共有コンピューターのライセンス認証に関する問題のトラブルシューティング](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="045e0-110">See [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
- <span data-ttu-id="045e0-111">「[Microsoft 365 Apps for enterprise のライセンス認証の状態をリセットする](https://go.microsoft.com/fwlink/?linkid=2109218)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="045e0-111">See [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="045e0-112">Microsoft 365 管理センターから Microsoft 365 Apps for enterprise を RDS にインストールする場合 (***既定のインストール設定を使用***) には、以下の手順を使用します。</span><span class="sxs-lookup"><span data-stu-id="045e0-112">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1.    <span data-ttu-id="045e0-113">契約しているサブスクリプションを確認します。</span><span class="sxs-lookup"><span data-stu-id="045e0-113">Check what subscription you have.</span></span> <span data-ttu-id="045e0-114">「[詳細](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="045e0-114">[Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2.    <span data-ttu-id="045e0-115">必要に応じて別のサブスクリプションに切り替えます。</span><span class="sxs-lookup"><span data-stu-id="045e0-115">If necessary, switch to a different subscription.</span></span> <span data-ttu-id="045e0-116">「[詳細](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="045e0-116">[Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span></span>
3.    <span data-ttu-id="045e0-117">他の Microsoft サブスクリプションを使用して Office が RDS サーバーに既にインストールされている場合には、アンインストールします。</span><span class="sxs-lookup"><span data-stu-id="045e0-117">If Office is already installed on the RDS server using any other Microsoft subscriptions, uninstall it.</span></span> <span data-ttu-id="045e0-118">たとえば、[**コントロール パネル**] >  [**プログラムのアンインストール**] の順に移動して行います。</span><span class="sxs-lookup"><span data-stu-id="045e0-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="045e0-119">問題が発生した場合には、[Microsoft サポート/回復アシスタント](https://aka.ms/SARA-OfficeUninstall-Alchemy)を使用してアンインストールしてください。</span><span class="sxs-lookup"><span data-stu-id="045e0-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4.    <span data-ttu-id="045e0-120">RDS サーバーで、管理者アカウントを使用して Microsoft 365 管理センターにサインインし、[Microsoft 365 Apps for enterprise をインストール](https://portal.office.com/OLS/MySoftware.aspx)します。</span><span class="sxs-lookup"><span data-stu-id="045e0-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5.    <span data-ttu-id="045e0-121">Office のインストール後は、Office アプリケーションを***開いたり、サインインしたりしないでください***。</span><span class="sxs-lookup"><span data-stu-id="045e0-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6.    <span data-ttu-id="045e0-122">RDS サーバーで、次の手順に従ってレジストリを編集し、共有コンピューターのライセンス認証を有効にします。</span><span class="sxs-lookup"><span data-stu-id="045e0-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="045e0-123">画面の左下隅にある Windows ボタンを右クリックし、[**実行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="045e0-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="045e0-124">[名前] ボックスに **regedit** と入力し、[**OK**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="045e0-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="045e0-125">レジストリ エディターがデバイスに変更を加えられるようにするかどうかを尋ねるプロンプトが表示されたら、[**はい**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="045e0-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="045e0-126">レジストリ エディターで、HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration に文字列値 **SharedComputerLicensing** を追加し、1 を設定します。</span><span class="sxs-lookup"><span data-stu-id="045e0-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="045e0-127">RDS サーバーで***エンド ユーザーとしてサインインし***、[共有コンピューターのライセンス認証が Microsoft 365 Apps for enterprise に対して有効になっていることを確認します](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)。</span><span class="sxs-lookup"><span data-stu-id="045e0-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

