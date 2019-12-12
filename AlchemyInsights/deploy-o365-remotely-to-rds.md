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
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>Office 365 ProPlus を展開して RDS、Terminal Server、または VDI で共有する

リモートデスクトップサービス (RDS) を使用して Office 365 ProPlus を展開するには、以前の名前付きターミナルサービスを使用します。
- Office 365 ProPlus (365 Office Enterprise E3、Enterprise E5 など) を含む、Microsoft 365 For Business プランまたは Office 365 プランを所有している必要があります。
   > [!NOTE] 
   > Office 365 Business および Office 365 Business Premium プランには、Office 365 ProPlus は含まれていません。
- [共有コンピューターのライセンス認証](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)を有効にする必要があります。

> [!NOTE]
> Office 365 ProPlus を共有コンピューターのライセンス認証モードでインストールするには、[Microsoft サポート/回復アシスタント](https://aka.ms/SaRA_OfficeSCA_M365Portal)をダウンロードして実行することもできます。

Office 展開ツールを使用してカスタマイズされたインストールの前提条件、セットアップ手順、およびガイダンスの詳細については、「 [Deploy office 365 ProPlus by Using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)」を参照してください。

共有コンピューターのライセンス認証に関連するエラーを修正するには、次のようにします。
- 「 [Office 365 ProPlus の共有コンピューターのライセンス認証に関する問題のトラブルシューティング](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)」を参照してください。
- 「 [Reset Office 365 ProPlus activation state](https://go.microsoft.com/fwlink/?linkid=2109218)」を参照してください。

***既定のインストール設定を使用***する Microsoft 365 管理センターから RDS に Office 365 ProPlus をインストールする場合は、次の手順を使用します。

1.  どの Office 365 プランを使用しているかを確認します。 [詳細情報](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)を参照してください。
2.  必要に応じて、別の Office 365 プランに切り替えます。 [詳細情報](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)を参照してください。
3.  Office が他の Office 365 プランを使用して RDS サーバーに既にインストールされている場合は、それをアンインストールします。 たとえば、[**コントロールパネル]** > を使用して**プログラムをアンインストール**します。 問題が発生している場合は[、Microsoft サポート/回復アシスタント](https://aka.ms/SARA-OfficeUninstall-Alchemy)を使用してアンインストールします。
4.  RDS サーバーで、管理者アカウントを使用して Microsoft 365 管理センターにサインインし、[Office 365 ProPlus をインストール](https://portal.office.com/OLS/MySoftware.aspx)します。
5.  Office のインストール後は、Office アプリケーションを***開いたり、サインインしたりしないでください***。
6.  RDS サーバーで、次の手順に従ってレジストリを編集し、共有コンピューターのライセンス認証を有効にします。
   1. 画面の左下隅にある [Windows] ボタンを右クリックし、[**実行**] を選択します。 [名前] ボックスに「 **regedit**」と入力し、[ **OK**] を選択します。
   2. レジストリエディターにデバイスの変更を許可するかどうかを確認するメッセージが表示されたら、[**はい**] を選択します。
   3. レジストリ エディターで、HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration に文字列値 **SharedComputerLicensing** を追加し、1 を設定します。
   4. RDS サーバーで***エンド ユーザーとしてサインインし***、[共有コンピューターのライセンス認証が Office 365 ProPlus に対して有効になっていることを確認します](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)。

