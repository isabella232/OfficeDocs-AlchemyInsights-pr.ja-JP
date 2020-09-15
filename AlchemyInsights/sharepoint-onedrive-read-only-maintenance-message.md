---
title: SharePoint または OneDrive を使用しようとすると、メンテナンスのため読み取り専用というメッセージが表示される場合
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670837"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>SharePoint または OneDrive を使用しようとすると、メンテナンスのため読み取り専用というメッセージが表示される場合

ユーザーが SharePoint または OneDrive を次のシナリオで使用しようとすると、**メンテナンスのため読み取り専用**というメッセージが表示される場合があります。 

-   予定されていたまたは実行中のメンテナンス アクティビティ。  [メッセージ センター](https://portal.office.com/adminportal/home#/messagecenter)に移動して、これらについて確認してください。
-   発生中の可能性がある、優先度の高いアクティブなサービス インシデント。 [サービス正常性](https://portal.office.com/adminportal/home#/servicehealth)に移動して、アドバイザリおよびインシデントを確認してください。
-   サーバー上での予期しないイベントが原因で発生中の可能性がある、継続時間が 30 分程度以内の軽微な自動復旧回復シナリオ。 
    
    これらの軽微な回復についてはメッセージ センターまたはサービス正常性に投稿されませんが、短時間で通常状態に回復します。

まれにですが、上記の 3 つのシナリオのいずれかが原因のケースで、サービスが回復したにも関わらずユーザーのブラウザーのキャッシュがクリアされないケースがあります。

ブラウザーのキャッシュをクリアしてから、サイトに移動してみてください。

1. Microsoft Edge ブラウザーで、[**設定**] を選択し、 [**プライバシーとセキュリティ**] を選択します。
2. [**閲覧データの消去**] で、[**クリアするデータの選択**] を選択します。
3. [**Cookies と保存済みの Web サイト データ**] を選択し、[**クリア**] を選択します。

>[!Note] 
> 注: 他のブラウザー (Mozilla Firefox や Google Chrome など) を使用している場合は、この手順とは異なる場合があります。

>[!Note] 
> 別の方法としては、新しい InPrivate ウィンドウで SharePoint サイトまたは OneDrive を開くこともできます。