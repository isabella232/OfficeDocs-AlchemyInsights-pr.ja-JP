---
title: SharePoint または OneDrive を使用しようとすると、メンテナンスのため読み取り専用というメッセージが表示される場合
ms.author: efrene
author: efrene
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
ms.openlocfilehash: cc232fba6f502e2b6f282a8c1a1e29221e36b70d
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840520"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>SharePoint または OneDrive を使用しようとすると、メンテナンスのため読み取り専用というメッセージが表示される場合

ユーザーが SharePoint または OneDrive を使用しようとすると、**メンテナンスのため読み取り専用**というメッセージが表示される場合があります。  これが表示された場合、[[メッセージ センター](https://portal.office.com/adminportal/home#/MessageCenter)] に移動して、テナントで進行中のメンテナンスがあるかどうかを確認してください。 また、[[サービス正常性](https://portal.office.com/adminportal/home#/servicehealth)] ダッシュボードを確認して、公開中のアドバイザリや発生中のインシデントがないかどうかを確認します。

[メッセージセンター] と [サービス正常性] ダッシュボードのどちらにも進行中のテナントのメンテナンスに関する情報がない場合、ブラウザー キャッシュの問題である可能性があります。

ブラウザーのキャッシュをクリアしてから、サイトに移動してみてください。

1. Microsoft Edge ブラウザーで、[**設定**] を選択し、 [**プライバシーとセキュリティ**] を選択します。
2. [**閲覧データの消去**] で、[**クリアするデータの選択**] を選択します。
3. [**Cookies と保存済みの Web サイト データ**] を選択し、[**クリア**] を選択します。

>[!Note] 
> 注: 他のブラウザー (Mozilla Firefox や Google Chrome など) を使用している場合は、この手順とは異なる場合があります。

>[!Note] 
> 別の方法としては、新しい InPrivate ウィンドウで SharePoint サイトまたは OneDrive を開くこともできます。