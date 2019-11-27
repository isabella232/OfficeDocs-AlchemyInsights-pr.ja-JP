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
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/15/2019
ms.locfileid: "37205414"
---
# <a name="installing-office-on-a-terminal-server"></a>ターミナル サーバーに Office をインストールする

リモート デスクトップ サービス (RDS、旧称ターミナル サービス) を使用して Office 365 ProPlus を Windows Server に展開する場合:
  
- Office 365 ProPlus を含む Office 365 プラン (Office 365 Enterprise E3 または Enterprise E5 など) が必要です。Office 365 Business プランと Office 365 Business Premium プランは、Office 365 ProPlus は含まれていません。

- [共有コンピューターのライセンス認証](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus)を有効にする必要があります。

Microsoft 365 管理センターから Office 365 ProPlus を RDS にインストールする場合 (***既定のインストール設定を使用***) は、次の手順を使用します。

> [!TIP]
> Office 365 ProPlus を共有コンピューターのライセンス認証モードでインストールするには、[Microsoft サポート/回復アシスタント](https://aka.ms/SaRA_OfficeSCA_M365Portal)をダウンロードして実行することもできます。
  
1. ご利用の Office 365 プランを確認します ([詳細](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have))。

2. 必要に応じて別の Office 365 プランに切り替えます ([詳細](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan))。

3. その他の Office 365 プランを使用して Office が RDS サーバーに既にインストールされている場合は、Office をアンインストールします。たとえば、[コントロール パネル] \> [プログラムのアンインストール] に移動します。問題が発生する場合は、[Microsoft サポート/回復アシスタント](https://aka.ms/SARA-OfficeUninstall-Alchemy)を使用してアンインストールします。

4. RDS サーバーで、管理者アカウントを使用して Microsoft 365 管理センターにサインインし、[Office 365 ProPlus をインストール](https://portal.office.com/OLS/MySoftware.aspx)します。

5. Office のインストール後は、Office アプリケーションを***開いたり、サインインしたりしないでください***。

6. RDS サーバーで、次の手順に従ってレジストリを編集し、共有コンピューターのライセンス認証を有効にします。

1. 画面左下隅の Windows ボタンを右クリックし、[実行] を選択します。[開く] ボックスに「**regedit**」と入力し、[OK] を選択します。

2. レジストリ エディターでデバイスを変更できるようにするかどうかを尋ねられたら、[はい] を選択します。

3. レジストリ エディターで、HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration に文字列値 **SharedComputerLicensing** を追加し、1 を設定します。

7. RDS サーバーで***エンド ユーザーとしてサインインし***、[共有コンピューターのライセンス認証が Office 365 ProPlus に対して有効になっていることを確認します](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)。

Office 展開ツールを使用したカスタム インストールの前提条件、設定手順、およびガイダンスの詳細については、「[リモート デスクトップ サービスを使用して Office 365 ProPlus を展開する](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)」を参照してください。
  
共有コンピューターのライセンス認証に関連するエラーを修正するには、「[Office 365 ProPlus に対する共有コンピューターのライセンス認証に関する問題のトラブルシューティング](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)」を参照してください。
  