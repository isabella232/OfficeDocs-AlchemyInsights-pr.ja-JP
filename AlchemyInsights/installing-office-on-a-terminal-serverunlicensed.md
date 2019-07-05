---
title: ターミナル サーバーに Office をインストールする - ライセンスなし
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 6fc4bd5f6971ca833084a6a8ad6c25b3fdafb8dc
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35381734"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="0ff1c-102">ターミナル サーバーに Office をインストールする</span><span class="sxs-lookup"><span data-stu-id="0ff1c-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="0ff1c-103">リモート デスクトップ サービス (RDS、旧称ターミナル サービス) を使用して Office 365 ProPlus を Windows Server に展開する場合:</span><span class="sxs-lookup"><span data-stu-id="0ff1c-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="0ff1c-p101">Office 365 ProPlus を含む Office 365 プラン (Office 365 Enterprise E3 または Enterprise E5 など) が必要です。Office 365 Business プランと Office 365 Business Premium プランは、Office 365 ProPlus は含まれていません。</span><span class="sxs-lookup"><span data-stu-id="0ff1c-p101">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5. The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="0ff1c-106">[共有コンピューターのライセンス認証](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)を有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="0ff1c-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="0ff1c-107">Office 365 ポータルから RDS に Office 365 ProPlus をインストールする場合 (\*\* *既定のインストール設定を使用* \*\*) は、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="0ff1c-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span>
  
1. <span data-ttu-id="0ff1c-p102">ご利用の Office 365 プランを確認します ([詳細](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have))。</span><span class="sxs-lookup"><span data-stu-id="0ff1c-p102">Check what Office 365 plan you have. [Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span></span>

2. <span data-ttu-id="0ff1c-p103">必要に応じて別の Office 365 プランに切り替えます ([詳細](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan))。</span><span class="sxs-lookup"><span data-stu-id="0ff1c-p103">If necessary, switch to a different Office 365 plan. [Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span></span>

3. <span data-ttu-id="0ff1c-p104">その他の Office 365 プランを使用して Office が RDS サーバーに既にインストールされている場合は、Office をアンインストールします。たとえば、[コントロール パネル] \> [プログラムのアンインストール] に移動します。問題が発生する場合は、[Microsoft サポート/回復アシスタント](https://aka.ms/SARA-OfficeUninstall-Alchemy)を使用してアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="0ff1c-p104">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it. For example, by going to Control Panel \> Uninstall a program. Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="0ff1c-115">RDS サーバーで、管理者アカウントを使用して Office 365 ポータルにサインインし、[Office 365 ProPlus をインストールします](https://portal.office.com/OLS/MySoftware.aspx)。</span><span class="sxs-lookup"><span data-stu-id="0ff1c-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="0ff1c-116">Office のインストール後には、Office アプリケーションを\*\* *開いたり、サインインしたりしないでください* \*\*。</span><span class="sxs-lookup"><span data-stu-id="0ff1c-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span>

6. <span data-ttu-id="0ff1c-117">RDS サーバーで、次の手順に従ってレジストリを編集し、共有コンピューターのライセンス認証を有効にします。</span><span class="sxs-lookup"><span data-stu-id="0ff1c-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="0ff1c-p105">画面左下隅の Windows ボタンを右クリックし、[実行] を選択します。[開く] ボックスに「**regedit**」と入力し、[OK] を選択します。</span><span class="sxs-lookup"><span data-stu-id="0ff1c-p105">Right-click the Windows button in the lower left-hand corner of your screen and select Run. In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="0ff1c-120">レジストリ エディターでデバイスを変更できるようにするかどうかを尋ねられたら、[はい] を選択します。</span><span class="sxs-lookup"><span data-stu-id="0ff1c-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="0ff1c-121">レジストリ エディターで、HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration に文字列値 **SharedComputerLicensing** を追加し、1 を設定します。</span><span class="sxs-lookup"><span data-stu-id="0ff1c-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="0ff1c-122">RDS サーバーで \*\* *エンド ユーザーとしてサインインし* \*\*、[共有コンピューターのライセンス認証が Office 365 ProPlus に対して有効になっていることを確認します](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)。</span><span class="sxs-lookup"><span data-stu-id="0ff1c-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="0ff1c-123">Office 展開ツールを使用したカスタム インストールの前提条件、設定手順、およびガイダンスの詳細については、「[リモート デスクトップ サービスを使用して Office 365 ProPlus を展開する](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0ff1c-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="0ff1c-124">共有コンピューターのライセンス認証に関連するエラーを修正するには、「[Office 365 ProPlus に対する共有コンピューターのライセンス認証に関する問題のトラブルシューティング](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0ff1c-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  