---
title: SharePoint Designer の接続に関する問題
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942030"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer の接続に関する問題 

SharePoint Designer で SharePoint サイトへの接続に問題が発生した場合は、次の一般的な解決方法を試してください。

手順 1: [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) および [SharePoint Designer 2013 の 2016 年 8 月 2 日の更新プログラム](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)を使用して SharePoint Designer 2013 が更新済みであることを確認します。



手順 2: ローカル キャッシュ ファイルをクリアします。

1. SharePoint Designer 2013 を閉じます。

2. ローカル コンピューターで、次の各フォルダーに含まれるファイルをすべて削除します。

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. SharePoint Designer 2013 を開いてもう一度アカウントにサインインし、動作を確認します。

手順 3: [Windows デバイスの Office 2013 の先進認証を有効にします](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)。

手順 4: SharePoint Designer 接続を可能にするために、管理者は SharePoint 管理センターの設定で、**カスタム スクリプトの実行を許可する** 必要があります。詳細については、「[カスタム スクリプトを許可または禁止する](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)」を参照してください。


