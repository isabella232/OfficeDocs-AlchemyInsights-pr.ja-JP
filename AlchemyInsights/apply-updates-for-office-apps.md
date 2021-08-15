---
title: Office アプリの更新を適用する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1747"
- "9000140"
ms.openlocfilehash: 418c1166560b33c445d7ec452caadaa2295b87cc4766e7d36b7d711abb81a48e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53969390"
---
# <a name="apply-updates-for-office-apps"></a>Office アプリの更新を適用する

既定では、Officeアプリの更新プログラムは無料で、自動的にダウンロードされ、ユーザーの介入なしにバックグラウンドで適用されます。 更新の適用で問題が発生した場合に手動で更新を実行するには、[「Office更新プログラムをインストールする」](https://support.office.com/article/install-office-updates-2ab296f3-7f03-43a2-8e50-46de917611c5)をご覧ください。 詳細については、[「Office インストール時のトラブルシューティング」](https://support.microsoft.com/office/troubleshoot-installing-office-35ff2def-e0b2-4dac-9784-4cf212c1f6c2?ui=en-us&rs=en-us&ad=us#O365Plans=signinorgid)をご覧ください。

ユーザーの Office 更新プログラムを管理するには、次のオプションを検討してください。

- 必要な更新頻度に基づいて、組織に合った Office 更新チャネルを選択してください。 方法については、[「 Microsoft 365 Apps の更新チャネルの概要」](https://docs.microsoft.com/deployoffice/overview-of-update-channels-for-office-365-proplus)を参照してください。

- 更新をインターネットから自動的に適用するか、オンプレミス共有から適用するかを決定します。 方法については、[「Microsoft 365 Apps の更新を管理する方法を選択する」](https://docs.microsoft.com/deployoffice/choose-how-to-manage-updates-to-office-365-proplus)を参照してください。

- 以下の手順で、Office の更新設定を確認し、更新がエンドユーザーのコンピューターにどう適用されるかを制御します。

    - [Microsoft 365 Apps の更新プログラム設定を構成します](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)。
    - [インストール後の Office の更新方法を指定します](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)。

Office アプリを複数のユーザーに展開する場合は、Office カスタマイズツールを使用して展開用の構成ファイルを作成し、Office 展開ツールを使用してOffice更新プログラムを構成します。 詳細については、「[Office カスタマイズツール](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)と [Office 展開ツールの概要](https://go.microsoft.com/fwlink/p/?LinkID=626065)」を参照してください。

- ユーザーグループをセットアップして Office 更新プログラムを展開する方法の例については、「[ローカル ソースから Microsoft 365 Apps を展開する](https://docs.microsoft.com/deployoffice/deploy-office-365-proplus-from-a-local-source)」を参照してください。
-   Office アプリが開いているために一部のユーザーに Office 更新プログラムが適用されない場合は、ForceAppShutdown 設定の使用を検討してください。 詳細については、[FORCEAPPSHUTDOWN プロパティ（プロパティ要素の一部）](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#forceappshutdown-property-part-of-property-element)を参照してください。 

**関連項目**

[Microsoft 365 Apps の更新プロセスの概要](https://docs.microsoft.com/deployoffice/overview-of-the-update-process-for-office-365-proplus)。  
[Microsoft 365 Apps の更新プログラムに関するリリース情報](https://docs.microsoft.com/officeupdates/release-notes-office365-proplus)。  
[Microsoft Endpoint Configuration Manager を使用して Microsoft 365 Apps の更新プログラムを管理する](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager)。  
