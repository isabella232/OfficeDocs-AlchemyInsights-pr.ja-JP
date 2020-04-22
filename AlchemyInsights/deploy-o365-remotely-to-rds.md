---
title: RDS、Terminal Server、または VDI で共有するために Microsoft 365 Apps for enterprise を展開する
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
ms.openlocfilehash: ddd44d40e9430ee31b8b734450dde0defef229d7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704710"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>RDS、Terminal Server、または VDI で共有するために Microsoft 365 Apps for enterprise を展開する

リモートデスクトップサービス (RDS) を使用してエンタープライズ向けの Microsoft 365 アプリを展開するには、以前の名前付きターミナルサービス:
- Office 365 Enterprise E3、Enterprise E5 など、エンタープライズ向け Microsoft 365 アプリを含む Microsoft 365 For Business プランまたは Office 365 プランが必要です。
   > [!NOTE] 
   > Microsoft 365 App for business および Microsoft 365 Business Premium Standard プランには、Microsoft 365 Apps for enterprise は含まれていません。
- [共有コンピューターのライセンス認証](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)を有効にする必要があります。

> [!NOTE]
> [Microsoft サポート/回復アシスタント](https://aka.ms/SaRA_OfficeSCA_M365Portal)をダウンロードして実行すると、共有コンピューターのライセンス認証モードで Microsoft 365 Apps for enterprise をインストールすることもできます。

Office 展開ツールを使用した、カスタマイズされたインストールの前提条件、セットアップ手順、およびガイダンスの詳細については、「 [Deploy Microsoft 365 Apps for enterprise by Using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)」を参照してください。

共有コンピューターのライセンス認証に関連するエラーを修正するには:
- 「 [Microsoft 365 Apps for enterprise での共有コンピューターのライセンス認証に関する問題のトラブルシューティング](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)」を参照してください。
- 「[Microsoft 365 Apps for enterprise のライセンス認証の状態をリセットする](https://go.microsoft.com/fwlink/?linkid=2109218)」を参照してください。

***既定のインストール設定を使用***する microsoft 365 管理センターから RDS に Microsoft 365 アプリをインストールする場合は、次の手順を実行します。

1.    ご使用のサブスクリプションを確認してください。 [詳細情報](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)を参照してください。
2.    必要に応じて、別のサブスクリプションに切り替えます。 [詳細情報](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)を参照してください。
3.    Office が他の Microsoft サブスクリプションを使用して RDS サーバーに既にインストールされている場合は、それをアンインストールします。 たとえば、[**コントロール パネル**] >  [**プログラムのアンインストール**] の順に移動して行います。 問題が発生した場合には、[Microsoft サポート/回復アシスタント](https://aka.ms/SARA-OfficeUninstall-Alchemy)を使用してアンインストールしてください。
4.    RDS サーバーで、管理者アカウントを使用して Microsoft 365 管理センターにサインインし、 [microsoft 365 Apps for enterprise をインストール](https://portal.office.com/OLS/MySoftware.aspx)します。
5.    Office のインストール後は、Office アプリケーションを***開いたり、サインインしたりしないでください***。
6.    RDS サーバーで、次の手順に従ってレジストリを編集し、共有コンピューターのライセンス認証を有効にします。
   1. 画面の左下隅にある Windows ボタンを右クリックし、[**実行**] を選択します。 [名前] ボックスに **regedit** と入力し、[**OK**] を選択します。
   2. レジストリ エディターがデバイスに変更を加えられるようにするかどうかを尋ねるプロンプトが表示されたら、[**はい**] を選択します。
   3. レジストリ エディターで、HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration に文字列値 **SharedComputerLicensing** を追加し、1 を設定します。
   4. RDS サーバーで、***エンドユーザーとしてサインイン***し、 [enterprise 用 Microsoft 365 アプリの共有コンピューターのライセンス認証が有効](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)になっていることを確認します。

