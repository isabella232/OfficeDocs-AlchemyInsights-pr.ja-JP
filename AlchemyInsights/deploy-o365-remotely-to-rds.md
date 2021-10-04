---
title: RDS、ターミナル サーバー、または VDI で共有して使用する Microsoft 365 Apps の展開
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
ms.openlocfilehash: 81183cf1823480c1b15eba9ba9f519b4e3746b52
ms.sourcegitcommit: ef8d6b71fbd962fb3f7081b21724e67a91111a92
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/01/2021
ms.locfileid: "60077255"
---
# <a name="deploying-microsoft-365-apps-for-shared-use-on-rds-terminal-server-or-vdi"></a>RDS、ターミナル サーバー、または VDI で共有して使用する Microsoft 365 Apps の展開

リモート デスクトップ サービス (RDS、旧称ターミナル サービス) を使用して Microsoft 365 Apps を展開するには、以下の操作を行う必要があります。

- 簡単な修正プログラムを使用して TLS 1.2 を既定として有効にし、以前のバージョンの Windows (Windows 7 SP1、Windows Server 2008 R2 など) を実行します。 簡単な修正プログラムや詳細については、「[Windows の WinHTTP で TLS 1.1 および TLS 1.2 を既定のセキュリティで保護されたプロトコルとして有効にするための更新プログラム](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy)」を参照してください。 
- Microsoft 365 Apps for enterprise (旧称 Office 365 Plus) を含むプランがあります。たとえば、Office 365 E3 や Microsoft 365 E5、Project Plan 3 や Visio Plan 2 などのデスクトップ版の Project や Visio を含むプラン、または Microsoft 365 Apps for business などの Microsoft 365 Business Premium プランです。
- 共有コンピューターのライセンス認証を有効にします。詳細は、「[Microsoft 365 Apps に対する共有コンピューターのライセンス認証の概要](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation)」をご覧ください。

**注**: 共有コンピューターのライセンス認証モードで Microsoft 365 Apps for enterprise をインストールするには、[Microsoft サポート/回復アシスタント](https://aka.ms/SaRA_OfficeSCA_M365Portal)をダウンロードして実行します。 Office 展開ツールを使用したカスタム インストールの前提条件、セットアップ手順、ガイダンスに関する詳細については、「[リモート デスクトップ サービスを使用して Microsoft 365 Apps を展開する](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services)」を参照してください。

共有コンピューターのライセンス認証に関連するエラーを修正するには、以下をご覧ください。

- [Microsoft 365 Apps に対する共有コンピューターのライセンス認証に関する問題のトラブルシューティング](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Microsoft 365 Apps for enterprise のライセンス認証の状態をリセットする](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Microsoft 365 管理センターから Microsoft 365 Apps を RDS にインストールする場合 (既定のインストール設定を使用) には、以下の手順に従ってください。

1. ご利用の Microsoft 365 プランを確認します。 詳細については、「[取得しているサブスクリプションが不明な場合](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)」をご覧ください。

1. 必要に応じて別の Microsoft 365 プランに切り替えます。 詳細については、「[別のプランにアップグレードする](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan)」を参照してください。

1. Microsoft 365 Apps が他の互換性のないプランを使用して既に RDS サーバーにインストールされている場合は、**[コントロール パネル]**、 > **[プログラムのアンインストール]** の順に移動してアンインストールします。 問題が発生した場合には、[Microsoft サポート/回復アシスタント](https://aka.ms/SARA-OfficeUninstall-Alchemy)をダウンロードしてアンインストールしてください。

1. RDS サーバーで、管理者アカウントを使用して Microsoft 365 管理センターにサインインし、[Office をインストール](https://portal.office.com/OLS/MySoftware.aspx)します。

   Office のインストール後は、Office アプリケーションを開いたり、サインインしたりしないでください。

1. RDS サーバーで、レジストリを編集し、共有コンピューターのライセンス認証を有効にします。

   1. 画面左下隅の Windows ボタンを右クリックし、**[実行]** を選択します。[開く] ボックスに「**regedit**」と入力し、**[OK]** を選択します。

   1. レジストリ エディターがデバイスに変更を加えられるようにするかどうかを尋ねるプロンプトが表示されたら、**[はい]** を選択します。

   1. レジストリ エディターで、HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration に文字列値 **SharedComputerLicensing** を追加し、**1** を設定します。

1. RDS サーバーでエンド ユーザーとしてサインインし、共有コンピューターのライセンス認証が Microsoft 365 Apps に対して有効になっていることを確認します。 

   詳細については、「[共有コンピューターのライセンス認証が Microsoft 365 Apps に対して有効になっていることを確認する](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps)」をご覧ください。