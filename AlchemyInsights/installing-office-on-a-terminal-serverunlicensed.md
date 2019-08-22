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
ms.openlocfilehash: edac051840594f13b22ccd83f5cd6e3da5f84cbc
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36498420"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="859fe-102">ターミナル サーバーに Office をインストールする</span><span class="sxs-lookup"><span data-stu-id="859fe-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="859fe-103">リモート デスクトップ サービス (RDS、旧称ターミナル サービス) を使用して Office 365 ProPlus を Windows Server に展開する場合:</span><span class="sxs-lookup"><span data-stu-id="859fe-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="859fe-p101">Office 365 ProPlus を含む Office 365 プラン (Office 365 Enterprise E3 または Enterprise E5 など) が必要です。Office 365 Business プランと Office 365 Business Premium プランは、Office 365 ProPlus は含まれていません。</span><span class="sxs-lookup"><span data-stu-id="859fe-p101">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5. The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="859fe-106">[共有コンピューターのライセンス認証](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)を有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="859fe-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="859fe-107">Office 365 ポータルから、***既定のインストール設定を使用***する Office 365 PROPLUS を RDS にインストールする場合は、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="859fe-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, ***which uses default installation settings***, follow these steps:</span></span>
  
1. <span data-ttu-id="859fe-p102">ご利用の Office 365 プランを確認します ([詳細](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have))。</span><span class="sxs-lookup"><span data-stu-id="859fe-p102">Check what Office 365 plan you have. [Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)</span></span>

2. <span data-ttu-id="859fe-p103">必要に応じて別の Office 365 プランに切り替えます ([詳細](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan))。</span><span class="sxs-lookup"><span data-stu-id="859fe-p103">If necessary, switch to a different Office 365 plan. [Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)</span></span>

3. <span data-ttu-id="859fe-p104">その他の Office 365 プランを使用して Office が RDS サーバーに既にインストールされている場合は、Office をアンインストールします。たとえば、[コントロール パネル] \> [プログラムのアンインストール] に移動します。問題が発生する場合は、[Microsoft サポート/回復アシスタント](https://aka.ms/SARA-OfficeUninstall-Alchemy)を使用してアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="859fe-p104">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it. For example, by going to Control Panel \> Uninstall a program. Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="859fe-115">RDS サーバーで、管理者アカウントを使用して Office 365 ポータルにサインインし、[Office 365 ProPlus をインストールします](https://portal.office.com/OLS/MySoftware.aspx)。</span><span class="sxs-lookup"><span data-stu-id="859fe-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="859fe-116">Office をインストールした後で、Office アプリケーションを***開いたりサインインしたりしない***でください。</span><span class="sxs-lookup"><span data-stu-id="859fe-116">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="859fe-117">RDS サーバーで、次の手順に従ってレジストリを編集し、共有コンピューターのライセンス認証を有効にします。</span><span class="sxs-lookup"><span data-stu-id="859fe-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="859fe-p105">画面左下隅の Windows ボタンを右クリックし、[実行] を選択します。[開く] ボックスに「**regedit**」と入力し、[OK] を選択します。</span><span class="sxs-lookup"><span data-stu-id="859fe-p105">Right-click the Windows button in the lower left-hand corner of your screen and select Run. In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="859fe-120">レジストリ エディターでデバイスを変更できるようにするかどうかを尋ねられたら、[はい] を選択します。</span><span class="sxs-lookup"><span data-stu-id="859fe-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="859fe-121">レジストリ エディターで、HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration に文字列値 **SharedComputerLicensing** を追加し、1 を設定します。</span><span class="sxs-lookup"><span data-stu-id="859fe-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="859fe-122">RDS サーバーで、***エンドユーザーとしてサインイン***し、 [Office 365 ProPlus で共有コンピューターのライセンス認証が有効になって](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)いることを確認します。</span><span class="sxs-lookup"><span data-stu-id="859fe-122">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="859fe-123">Office 展開ツールを使用したカスタム インストールの前提条件、設定手順、およびガイダンスの詳細については、「[リモート デスクトップ サービスを使用して Office 365 ProPlus を展開する](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="859fe-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="859fe-124">共有コンピューターのライセンス認証に関連するエラーを修正するには、「[Office 365 ProPlus に対する共有コンピューターのライセンス認証に関する問題のトラブルシューティング](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="859fe-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  