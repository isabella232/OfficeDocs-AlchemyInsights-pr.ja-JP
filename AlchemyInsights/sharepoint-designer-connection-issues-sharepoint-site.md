---
title: SharePoint Online のアクセス許可レベル
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "35086087"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer の接続に関する問題 

SharePoint Designer で SharePoint サイトへの接続に問題が発生した場合は、次の一般的な解決方法を試してください。

手順 1: SharePoint Designer が更新されていることを確認する。

- [SharePoint Designer 2013](https://www.microsoft.com/download/details.aspx?id=35491)

- [SharePoint Designer Service Pack 1 (SP1)](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [SharePoint Designer 2013 の更新プログラム (KB3114721)](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

手順 2: ローカル キャッシュ ファイルをクリアする

- SharePoint Designer 2013 を閉じます。

- ローカル コンピューターで、次のフォルダーを参照してキャッシュされているファイルを削除します。

- [スタート]、[実行] の順にクリックして、次の各場所にあるすべてのファイルを削除します。

%APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

SharePoint Designer 2013 を開いて、動作を確認するために、もう一度アカウントを入力します。

手順 3: [Windows デバイスの Office 2013 の先進認証を有効にする](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

手順 4: 管理者は SharePoint Designer の接続を可能にするカスタム スクリプトの実行を許可する必要があります。

詳細な手順、例、および考慮事項については、「[カスタム スクリプトを許可または禁止する](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)」を参照してください。


