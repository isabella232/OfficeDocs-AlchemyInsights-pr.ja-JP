---
title: ターミナル サーバーに Office をインストールする - ライセンスなし
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 35ef317ea87fedd01c08fee5b370e3c81e515c27
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322004"
---
# <a name="installing-office-on-a-terminal-server"></a>ターミナル サーバーに Office をインストールする

リモート デスクトップ サービス (RDS、旧称ターミナル サービス) を使用して Microsoft 365 Apps for enterprise を Windows Server に展開する場合:
  
- Microsoft 365 Apps for enterprise を含む Microsoft 365 サブスクリプション (Office 365 Enterprise E3、Enterprise E5 など) が必要です。 Microsoft 365 Apps for business と Microsoft 365 Apps for business Premium プランには Microsoft 365 Apps for enterprise は含まれていません。

- 
            [共有コンピューターのライセンス認証](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)を有効にする必要があります。

Microsoft 365 管理センターから Microsoft 365 Apps for enterprise を RDS にインストールする場合 (***既定のインストール設定を使用***) には、以下の手順を使用します。

    **Tip**: You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.
  
1. Microsoft 365 サブスクリプションを確認してください。[詳細情報](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. 必要に応じて、別の Microsoft 365 サブスクリプションに切り替えます。[詳細情報](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. その他の Microsoft 365 サブスクリプションを使用して Office が RDS サーバーに既にインストールされている場合は、Office をアンインストールします。たとえば、[コントロール パネル] \> [プログラムのアンインストール] に移動します。問題が発生する場合は、[Microsoft サポート/回復アシスタント](https://aka.ms/SARA-OfficeUninstall-Alchemy)を使用してアンインストールします。

4. RDS サーバーで、管理者アカウントを使用して Microsoft 365 管理センターにサインインし、[Microsoft 365 Apps for enterprise をインストール](https://portal.office.com/OLS/MySoftware.aspx)します。

5. Office のインストール後は、Office アプリケーションを ***開いたり、サインインしたりしないでください***。

6. RDS サーバーで、次の手順に従ってレジストリを編集し、共有コンピューターのライセンス認証を有効にします。

1. 画面左下隅の Windows ボタンを右クリックし、[実行] を選択します。[開く] ボックスに「**regedit**」と入力し、[OK] を選択します。

2. レジストリ エディターでデバイスを変更できるようにするかどうかを尋ねられたら、[はい] を選択します。

3. レジストリ エディターで、HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration に文字列値 **SharedComputerLicensing** を追加し、1 を設定します。

7. RDS サーバーで ***エンド ユーザーとしてサインインし***、[共有コンピューターのライセンス認証が Microsoft 365 Apps for enterprise に対して有効になっていることを確認します](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)。

Office 展開ツールを使用したカスタム インストールの前提条件、セットアップ手順、ガイダンスについて詳しくは、「[リモート デスクトップ サービスを使用して Microsoft 365 Apps for enterprise を展開する](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)」を参照してください。
  
共有コンピューターのライセンス認証に関連するエラーを修正するには、「[Microsoft 365 Apps for enterprise に対する共有コンピューターのライセンス認証に関する問題のトラブルシューティング](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)」を参照してください。
  