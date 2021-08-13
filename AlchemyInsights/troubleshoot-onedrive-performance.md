---
title: OneDrive のパフォーマンスのトラブルシューティング
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 15d9067e6b55b91af312671db9209f93ffc58859aaf69d63c84dbc354aff3dd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939132"
---
# <a name="troubleshoot-onedrive-performance"></a>OneDrive のパフォーマンスのトラブルシューティング

予想よりも遅い同期が発生している場合、または OneDrive に同様のパフォーマンスの問題が発生している場合:

- [サービスの正常性ダッシュボード](https://portal.office.com/adminportal/home?ref=/servicehealth)を使用して、既知の問題がないことを確認します。

- OneDrive のファイルをすべてダウンロードし、デバイス上の記憶域を使用することなく、すべてのファイルにアクセスできるようにするために、[ファイル オンデマンド機能を有効にします](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e)。

- ネットワーク計画とパフォーマンスの[ベスト プラクティスを確認します](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance)。

- 特にデバイスを初めて同期する場合は、[アップロードとダウンロードの速度を最大化します](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43)。

- 10 万件を超えるアイテムを含むライブラリを同期している場合、OneDrive の同期が長時間停止しているように見えるか、状態に "xMB の 0KB を処理中" と表示される可能性があります。 [詳細については、「10 万件を超えるファイルの同期」](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa)および[「OneDrive でサポートされる 30 万ファイルの上限」](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa)を参照してください。

- あるユーザーが使用制限を超えると、そのユーザー アカウントからさらに送られる要求は SharePoint Online によって短時間、調整されます。調整が有効な間、ユーザー操作はすべて調整されます。
