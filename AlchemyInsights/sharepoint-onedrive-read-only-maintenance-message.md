---
title: 127 メールにアクセスしようとしたときに TenantAccessBlockedException エラーが表示される場合
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 5613138e7613deb264a7ab2c966f8b9c4a24763d
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/05/2019
ms.locfileid: "35174432"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>SharePoint または OneDrive を使用しようとした場合に、メンテナンスメッセージの読み取り専用にする

ユーザーが SharePoint または OneDrive を使用しようとすると、メンテナンスメッセージの読み取り専用のメッセージが表示されることがあります。

[メッセージセンター](https://portal.office.com/adminportal/home#/MessageCenter)に移動して、テナントでアクティブなメンテナンスが発生しているかどうかを確認します。 最後に、[[サービス正常性](https://portal.office.com/adminportal/home#/servicehealth)] ページにアクセスして、発生している可能性があるすべてのアドバイザリ/インシデントを確認してください。

メッセージセンターまたはサービス正常性ダッシュボードで、テナントの現在のメンテナンスについての情報がない場合は、ブラウザーのキャッシュの問題である可能性があります。

サイトに移動する前に、ブラウザーのキャッシュをクリアしてください。

- Microsoft Edge ブラウザーで、[詳細設定] に移動します。

- [ブラウズをクリアする] で、[削除対象を選択する] を選択します。
- [Cookie と保存された web サイトデータ] チェックボックスをオンにして、[クリア] を選択します。

**注**: Firefox や Chrome などの他のブラウザーを使用する場合、これらの手順は異なる場合があります。

