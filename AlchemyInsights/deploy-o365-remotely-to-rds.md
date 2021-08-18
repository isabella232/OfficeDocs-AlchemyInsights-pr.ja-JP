---
title: RDS、ターミナル サーバー、または VDI で共有して使用する Microsoft 365 Apps for enterprise の展開
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: b8df97c19937a757c1de9865b6c7b8d1cddfd62d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325608"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>RDS、ターミナル サーバー、または VDI で共有して使用する Microsoft 365 Apps for enterprise の展開

リモート デスクトップ サービス (RDS、旧称ターミナル サービス) を使用して Microsoft 365 Apps for enterprise を展開するには:

- Microsoft 365 For Business プラン、あるいは Microsoft 365 Apps for enterprise を含む Office 365 プラン (Office 365 Enterprise E3、Enterprise E5 など) が必要です。
   **注**: Microsoft 365 Apps for business と Microsoft 365 Business Standard プランには Microsoft 365 Apps for enterprise が含まれていません。
- [共有コンピューターのライセンス認証](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)を有効にする必要があります。

**注**: [Microsoft サポート/回復アシスタント](https://aka.ms/SaRA_OfficeSCA_M365Portal)をダウンロードして実行することによっても、Microsoft 365 Apps for enterprise を共有コンピューターのライセンス認証モードでインストールできます。

Office 展開ツールを使用したカスタム インストールの前提条件、セットアップ手順、ガイダンスについて詳しくは、「[リモート デスクトップ サービスを使用して Microsoft 365 Apps for enterprise を展開する](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)」を参照してください。

共有コンピューターのライセンス認証に関連するエラーを修正するには:

- 「[Microsoft 365 Apps for enterprise に対する共有コンピューターのライセンス認証に関する問題のトラブルシューティング](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)」を参照してください。
- 「[Microsoft 365 Apps for enterprise のライセンス認証の状態をリセットする](https://go.microsoft.com/fwlink/?linkid=2109218)」を参照してください。

Microsoft 365 管理センターから Microsoft 365 Apps for enterprise を RDS にインストールする場合 (***既定のインストール設定を使用***) には、以下の手順を使用します。

1. 契約しているサブスクリプションを確認します。[方法はこちら](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)。
2. 必要に応じて別のサブスクリプションに切り替えます。[方法はこちら](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)。
3. その他の Microsoft サブスクリプションを使用して Office が RDS サーバーに既にインストールされている場合は、Office をアンインストールします。たとえば、**[コントロール パネル]** > **[プログラムのアンインストール]** に移動します。問題が発生する場合は、[Microsoft サポート/回復アシスタント](https://aka.ms/SARA-OfficeUninstall-Alchemy)を使用してアンインストールします。
4. RDS サーバーで、管理者アカウントを使用して Microsoft 365 管理センターにサインインし、[Microsoft 365 Apps for enterprise をインストール](https://portal.office.com/OLS/MySoftware.aspx)します。
5. Office のインストール後は、Office アプリケーションを ***開いたり、サインインしたりしないでください***。
6. RDS サーバーで、次の手順に従ってレジストリを編集し、共有コンピューターのライセンス認証を有効にします。
   1. 画面左下隅の Windows ボタンを右クリックし、[**実行**] を選択します。[開く] ボックスに「**regedit**」と入力し、[**OK**] を選択します。
   2. レジストリ エディターがデバイスに変更を加えられるようにするかどうかを尋ねるプロンプトが表示されたら、[**はい**] を選択します。
   3. レジストリ エディターで、HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration に文字列値 **SharedComputerLicensing** を追加し、1 を設定します。
   4. RDS サーバーで ***エンド ユーザーとしてサインインし***、[共有コンピューターのライセンス認証が Microsoft 365 Apps for enterprise に対して有効になっていることを確認します](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)。
