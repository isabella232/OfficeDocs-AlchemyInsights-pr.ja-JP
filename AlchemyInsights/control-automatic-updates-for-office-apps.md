---
title: Officeアプリの自動更新を制御する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440564"
---
# <a name="control-automatic-updates-for-office-apps"></a>Officeアプリの自動更新を制御する

既定では、Office アプリの更新は自動的にダウンロードされ、ユーザーの介入なしにバックグラウンドで適用されます。 ただし、管理者は Office 更新プログラムの設定を使用して、更新の適用方法を制御できます。 更新設定で、管理者は自動更新を有効または無効にしたり、Officeの **[今すぐ更新する]** ボタンを表示または非表示にしたり、更新の期限を設定したりできます。 詳細については、次を参照してください。

- [Office の更新設定を構成する](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Office の自動更新が有効になっていません](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [インストール後の Office の更新方法を指定する](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

クライアント マシンに適用されている既存の更新設定を確認するには、次の手順を実行します。

1. **Start** > **Run** > **Regedit** に移動して、レジストリエディタを開きます。
2. 以下の場所に移動し、Office の更新プログラムの設定を確認します。  
    a.  HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\  
    b.  ClickToRun\Configuration

**注** OfficeMgmtCOM キーが設定されている場合、**Office** > **アカウント** > **Office Updates**に「システム管理者によって更新が管理されています」というメッセージが表示される場合があります。 詳細は、「[Microsoft Endpoint Configuration Manager を使用して Microsoft 365 Apps の更新プログラムを管理する](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager)」をご覧ください。  