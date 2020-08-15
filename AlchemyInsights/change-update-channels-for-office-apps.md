---
title: Office アプリの更新プログラム チャネルを変更する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 3e1042a38d2289b9ef2396e8300d32f20ddaa703
ms.sourcegitcommit: b5e5f560bf6ef92b4475bd3d91b7df38b5a4b036
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/14/2020
ms.locfileid: "46739832"
---
# <a name="change-update-channels-for-office-apps"></a>Office アプリの更新プログラム チャネルを変更する

新しい Office をインストールする場合は、Office ソフトウェアのダウンロード設定を使用して目的の更新プログラム チャネルを選び、Office アプリをインストール (または再インストール) します。 詳細については、[「Office 365 のソフトウェア ダウンロードの設定を管理する」](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365) をご覧ください。 

**注** Office のソフトウェア ダウンロードの設定を使用して選択された更新プログラム チャネルは、O365 ポータルを使用して新しいインストールを実行しているすべてのユーザーに適用されます。 詳細については、[「Microsoft 365 または Office 2019 を PC または Mac にダウンロードしてインストールまたは再インストールする」](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658) を参照してください。   

既存の Office インストールの場合、Office 展開ツール (ODT) を使用して別の更新プログラム チャネルに切り替えます:  

1. [Microsoft ダウンロード センター](https://go.microsoft.com/fwlink/p/?LinkID=626065) から最新バージョンの Office 展開ツール (setup.exe) をダウンロードします。
2. 切り替えるチャネルの名前を指定します。 詳細については、[「Office 展開ツールの構成オプション」](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element) を参照してください。
3. 適切なチャネル名 (たとえば、update.xml) を指定する構成 XML ファイルを作成します。  

`<Configuration>`<br>
`<Updates Channel="Monthly"/>`<br>
`</Configuration>`<br>

4. 管理者特権のコマンド プロンプトから、setup.exe が置かれているフォルダーに切り替え、次のコマンドを実行します:  
    a.  setup.exe /configure update.xml
5. Office アプリケーション (Excel など) を起動し、**[ファイル]** > **[アカウント]** の順に選択します。 [製品情報] セクションで、**[更新オプション]** > **[今すぐ更新]** の順に選択します。

詳細については、[「既存の Office アプリの更新プログラム チャネルを切り替える方法」](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel) を参照してください。 

選択したユーザーのグループまたは構成マネージャー (SCCM) を使用して更新プログラム チャネルを切り替えるには、GPO を使用して更新プログラム チャネルの設定を構成します。 詳細については、[「Microsoft 365 アプリの更新プログラム チャネルの概要」](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy) を参照してください。 詳細については、[「IT 担当者向け Office 365 ProPlus チャネルを管理する方法」](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813)、[「Microsoft Endpoint Configuration Manager を使用して Microsoft 365 アプリの更新を管理する」](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager) を参照してください。