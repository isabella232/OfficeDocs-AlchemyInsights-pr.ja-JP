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
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/05/2019
ms.locfileid: "35174432"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>SharePoint または OneDrive を使用しようとすると、読み取り専用のメンテナンス メッセージが表示される場合

ユーザーが SharePoint または OneDrive を使用しようとすると、読み取り専用のメンテナンス メッセージが表示される場合。

[[メッセージ センター]](https://portal.office.com/adminportal/home#/MessageCenter) に移動して、テナントでアクティブ メンテナンスが実施されているかどうかを確認してください。 最後に、[サービス正常性](https://portal.office.com/adminportal/home#/servicehealth) ページにアクセスして、発生している可能性のあるアドバイザリ/インシデントを確認してください。

メッセージセンターまたはサービス正常性ダッシュボードに、テナントの現在のメンテナンス情報がない場合、ブラウザーキャッシュの問題である可能性があります。

ブラウザーのキャッシュをクリアしてから、サイトに移動してみてください。

- Microsoft Edge ブラウザーで、[その他...] > [設定] に移動します

- [閲覧データのクリア] で、[クリアするデータの選択] を選択します。
- [Cookie と保存済みの Web サイト データ] チェック ボックスをオンにして、[クリア] を選択します。

**注**: 別のブラウザー (Firefox や Chrome など) を使用している場合は、この手順とは異なる場合があります。

