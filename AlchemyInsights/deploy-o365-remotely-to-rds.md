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
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>RDS、ターミナル サーバー、または VDI での共有使用のための Office 365 ProPlus の展開

リモート デスクトップ サービス (RDS、旧称ターミナル サービス) を使用して Office 365 ProPlus を展開するには:
- Microsoft 365 For Business プラン、または Office 365 Enterprise E3 や Enterprise E5 などの Office 365 ProPlus を含む Office 365 プランが必要です。
   > [!NOTE] 
   > Office 365 Business および Office 365 Business Premium プランには、Office 365 ProPlus は含まれません。
- [共有コンピューターのライセンス認証](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)を有効にする必要があります。

> [!NOTE]
> Office 365 ProPlus を共有コンピューターのライセンス認証モードでインストールするには、[Microsoft サポート/回復アシスタント](https://aka.ms/SaRA_OfficeSCA_M365Portal)をダウンロードして実行することもできます。

前提条件の詳細、セットアップ手順、および Office 展開ツールを使用したカスタマイズされたインストールのガイダンスについては、「[リモート デスクトップ サービスを使用して Office 365 ProPlus を展開する](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)」を参照してください。

共有コンピューターのライセンス認証に関連するエラーを修正するには:
- [Office 365 ProPlus に対する共有コンピューターのライセンス認証に関する問題のトラブルシューティング](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)をご覧ください。
- 「[Office 365 ProPlus のライセンス認証の状態をリセットする](https://go.microsoft.com/fwlink/?linkid=2109218)」をご覧ください。

Microsoft 365 管理センターから Office 365 ProPlus を RDS にインストールする場合 (***既定のインストール設定を使用***) には、以下の手順を使用します。

1.  ご利用の Office 365 プランを確認します。 [詳細情報](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)を参照してください。
2.  必要に応じて別の Office 365 プランに切り替えます。 [詳細情報](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)を参照してください。
3.  他の Office 365 プランを使用して Office が RDS サーバーに既にインストールされている場合には、アンインストールします。 たとえば、[**コントロール パネル**] >  [**プログラムのアンインストール**] の順に移動して行います。 問題が発生した場合には、[Microsoft サポート/回復アシスタント](https://aka.ms/SARA-OfficeUninstall-Alchemy)を使用してアンインストールしてください。
4.  RDS サーバーで、管理者アカウントを使用して Microsoft 365 管理センターにサインインし、[Office 365 ProPlus をインストール](https://portal.office.com/OLS/MySoftware.aspx)します。
5.  Office のインストール後は、Office アプリケーションを***開いたり、サインインしたりしないでください***。
6.  RDS サーバーで、次の手順に従ってレジストリを編集し、共有コンピューターのライセンス認証を有効にします。
   1. 画面の左下隅にある Windows ボタンを右クリックし、[**実行**] を選択します。 [名前] ボックスに **regedit** と入力し、[**OK**] を選択します。
   2. レジストリ エディターがデバイスに変更を加えられるようにするかどうかを尋ねるプロンプトが表示されたら、[**はい**] を選択します。
   3. レジストリ エディターで、HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration に文字列値 **SharedComputerLicensing** を追加し、1 を設定します。
   4. RDS サーバーで***エンド ユーザーとしてサインインし***、[共有コンピューターのライセンス認証が Office 365 ProPlus に対して有効になっていることを確認します](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)。

