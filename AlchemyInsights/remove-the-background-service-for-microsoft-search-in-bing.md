---
title: Bing での Microsoft Search のバックグラウンド サービスを削除する
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816526"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Bing での Microsoft Search のバックグラウンド サービスを削除する

Bing での Microsoft Search のバックグラウンド サービスを削除するには、次の対処法を試すことができます。

1. 検索エンジンの設定を元に戻すには、次のようにします。

    a. **Bing を既定の検索エンジンとして使用する[トグルを](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)オフ** に切り替えます。

    b. [Microsoft 365 管理センターに移動](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed)し、組織内の全ユーザーに影響する設定を解除します。

2. 個人のデバイスからバックグラウンド サービスを削除するには、次のタスクを実行します。

    a. **[コントロール パネル] > [プログラム] > [プログラムと機能]** の順に選択します。

    b. 現在インストールされているプログラムのリストで、**[Bing での Microsoft Search]**] を右クリックし、**[アンインストール]** をクリックします。

3. 組織内の複数のデバイスからバックグラウンド サービスを削除するには、管理者としてログインし、スクリプトで次のコマンドを実行します。 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
