---
title: ターミナル サーバーに Office をインストールする - ライセンスなし
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: c781e9fd492ff97bc80667956e6609b3d40b28b4
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508633"
---
# <a name="installing-office-on-a-terminal-server"></a>ターミナル サーバーに Office をインストールする

リモート デスクトップ サービス (RDS、旧称ターミナル サービス) を使用して Microsoft 365 Apps for enterprise を Windows Server に展開する場合:
  
- Microsoft 365 Apps for enterprise を含む Microsoft 365 サブスクリプション (Office 365 Enterprise E3、Enterprise E5 など) が必要です。 Microsoft 365 Apps for business と Microsoft 365 Apps for business Premium プランには Microsoft 365 Apps for enterprise は含まれていません。

- 
            [共有コンピューターのライセンス認証](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)を有効にする必要があります。

Microsoft 365 管理センターから Microsoft 365 Apps for enterprise を RDS にインストールする場合 (***既定のインストール設定を使用***) には、以下の手順を使用します。

> [!TIP]
> [Microsoft サポート/回復アシスタント](https://aka.ms/SaRA_OfficeSCA_M365Portal)をダウンロードして実行することによっても、Microsoft 365 Apps for enterprise を共有コンピューターのライセンス認証モードでインストールできます。
  
1. Check what Microsoft 365 subscription you have. [Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. If necessary, switch to a different Microsoft 365 subscription. [Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it. For example, by going to Control Panel \> Uninstall a program. Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.

4. RDS サーバーで、管理者アカウントを使用して Microsoft 365 管理センターにサインインし、[Microsoft 365 Apps for enterprise をインストール](https://portal.office.com/OLS/MySoftware.aspx)します。

5. Office のインストール後は、Office アプリケーションを***開いたり、サインインしたりしないでください***。

6. RDS サーバーで、次の手順に従ってレジストリを編集し、共有コンピューターのライセンス認証を有効にします。

1. Right-click the Windows button in the lower left-hand corner of your screen and select Run. In the Open box, type **regedit**, and then select OK.

2. レジストリ エディターでデバイスを変更できるようにするかどうかを尋ねられたら、[はい] を選択します。

3. レジストリ エディターで、HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration に文字列値 **SharedComputerLicensing** を追加し、1 を設定します。

7. RDS サーバーで***エンド ユーザーとしてサインインし***、[共有コンピューターのライセンス認証が Microsoft 365 Apps for enterprise に対して有効になっていることを確認します](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)。

Office 展開ツールを使用したカスタム インストールの前提条件、セットアップ手順、ガイダンスについて詳しくは、「[リモート デスクトップ サービスを使用して Microsoft 365 Apps for enterprise を展開する](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)」を参照してください。
  
共有コンピューターのライセンス認証に関連するエラーを修正するには、「[Microsoft 365 Apps for enterprise に対する共有コンピューターのライセンス認証に関する問題のトラブルシューティング](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)」を参照してください。
  