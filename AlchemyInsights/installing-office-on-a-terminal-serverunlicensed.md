---
title: ターミナル サーバーのライセンスで office をインストールします。
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 73d5128b55cae7712c48be9e2d05e558c3ba2e5c
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29477109"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="11e20-102">ターミナル サーバーに Office をインストールします。</span><span class="sxs-lookup"><span data-stu-id="11e20-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="11e20-103">Office 365 用リソースのリモート デスクトップ サービス (RDS) を使用して、Windows サーバーを展開する、以前という名前のターミナル サービス。</span><span class="sxs-lookup"><span data-stu-id="11e20-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="11e20-p101">Office 365 用リソース、Office 365 エンタープライズ E3、E5 の企業などを含む、Office 365 のプランが必要です。Office 365 のビジネスと Office 365 のビジネス プレミアム プランは、Office 365 用リソースに含めないでください。</span><span class="sxs-lookup"><span data-stu-id="11e20-p101">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5. The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
    
- <span data-ttu-id="11e20-106">[共有のコンピューターのライセンス認証](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)を有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="11e20-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>
    
<span data-ttu-id="11e20-107">Office 365 ポータルから RDS に、Office 365 用リソースをインストールする場合は、\* **既定のインストール設定を使用する** \*、これらの手順に従います。</span><span class="sxs-lookup"><span data-stu-id="11e20-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span> 
  
1. <span data-ttu-id="11e20-p102">あるどのような Office 365 のプランを確認してください。[についてはどのように](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span><span class="sxs-lookup"><span data-stu-id="11e20-p102">Check what Office 365 plan you have. [Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span></span>
    
2. <span data-ttu-id="11e20-p103">必要に応じて、別の Office 365 に切り替える予定がある場合。[についてはどのように](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span><span class="sxs-lookup"><span data-stu-id="11e20-p103">If necessary, switch to a different Office 365 plan. [Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span></span>
    
3. <span data-ttu-id="11e20-p104">場合は、他の Office 365 のプランを使用して RDS サーバーには、Office が既にインストールされて、それをアンインストールします。コントロール パネルで、\>プログラムをアンインストールします。問題が発生している場合は、[マイクロソフトのサポートと回復時のアシスタント](https://aka.ms/SARA-OfficeUninstall-Alchemy)を使用してアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="11e20-p104">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it. For example, by going to Control Panel \> Uninstall a program. Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span> 
    
4. <span data-ttu-id="11e20-115">RDS サーバーで、管理者アカウントと[Office 365 用リソースのインストール](https://portal.office.com/OLS/MySoftware.aspx)と Office 365 ポータルにサインインします。</span><span class="sxs-lookup"><span data-stu-id="11e20-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
    
5. <span data-ttu-id="11e20-116">Office をインストールすると、\* **を開くまたはにサインインしない** \* すべての Office アプリケーションにします。</span><span class="sxs-lookup"><span data-stu-id="11e20-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span> 
    
6. <span data-ttu-id="11e20-117">RDS サーバーで、次の手順でレジストリを編集することによって共有されているコンピューターのライセンス認証を有効にします。</span><span class="sxs-lookup"><span data-stu-id="11e20-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
    
1. <span data-ttu-id="11e20-p105">画面の左下隅の [Windows] ボタンを右クリックし、[実行] を選択します。[名前] ボックスに**regedit**と入力し、[ok] を選択します。</span><span class="sxs-lookup"><span data-stu-id="11e20-p105">Right-click the Windows button in the lower left-hand corner of your screen and select Run. In the Open box, type **regedit**, and then select OK.</span></span> 
    
2. <span data-ttu-id="11e20-120">選択 [はい] レジストリ エディターを許可するメッセージが表示されたら、デバイスを変更するのにします。</span><span class="sxs-lookup"><span data-stu-id="11e20-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>
    
3. <span data-ttu-id="11e20-121">レジストリ エディターでは、HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration の下に 1 を設定すると**SharedComputerLicensing**の文字列値を追加します。</span><span class="sxs-lookup"><span data-stu-id="11e20-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span> 
    
7. <span data-ttu-id="11e20-122">RDS サーバーでは、\* \* *、エンド ・ ユーザーとしてサインイン*\* \* [Office 365 用リソースの共有のコンピューターのライセンス認証が有効になっている](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)ことを確認します。</span><span class="sxs-lookup"><span data-stu-id="11e20-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>
    
<span data-ttu-id="11e20-123">前提条件、セットアップ方法について説明し、このガイドには、Office の展開ツールを使用してインストールをカスタマイズの詳細についてを参照してください[展開 Office 365 用リソースがリモート デスクトップ サービスを使用して](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)ください。</span><span class="sxs-lookup"><span data-stu-id="11e20-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="11e20-124">共有のコンピューターのライセンス認証に関連するエラーを修正するのには、 [Office 365 用リソースの共有のコンピューターのライセンス認証の問題のトラブルシューティング](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="11e20-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  

