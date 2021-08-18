---
title: SharePoint ライブラリをネットワーク ドライブにマップする
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
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: 741d22c4231886b385b0bc2361e429929ef58f4b84d56e51186f129fc5d07921
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/11/2021
ms.locfileid: "57901593"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a>SharePoint ライブラリをネットワーク ドライブにマップする

ネットワーク ドライブをマップする代わりに、ファイル オンデマンド機能が備わった新しい OneDrive 同期クライアントを使用して SharePoint ファイルを同期します。 OneDrive 内のすべてのファイルに、ローカル記憶域を使用することなくアクセスできます。 詳細については、「[SharePoint および Teams のファイルをコンピューターと同期する](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88)」および「[Windows 10 用 OneDrive ファイル オンデマンドでディスク領域を節約する](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e)」を参照してください。

[新しい OneDrive 同期クライアント](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88)を使用する代わりにドライブをマップする場合は、以下の手順に従ってください。

- [SharePoint Online に接続するマップされたネットワーク ドライブのトラブルシューティング](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)

- [クライアントが TLS 1.2 をサポートしていないときに、認証エラーが発生する](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support#network-drive-mapped-to-a-sharepoint-library)  

**注:** Windows 8 または Windows 7 で実行する Internet Explorer 10 でドライブをマップする際に "**アクセスが拒否されました**" または "**パスにアクセスできません**" というメッセージが表示される場合は、この [修正プログラム](https://support.microsoft.com/topic/error-when-you-open-a-sharepoint-document-library-in-windows-explorer-or-map-a-network-drive-to-the-library-after-you-install-internet-explorer-10-96e640ba-059f-9b09-bb91-2a0319ee8b1d)をインストールして問題を解決してください。