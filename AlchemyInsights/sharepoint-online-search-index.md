---
title: SharePoint Online の検索辞書を管理する
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 5319c2f1edc3e61074301f039736d2aa96bda47b
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "35174468"
---
# <a name="search-in-sharepoint-online"></a>SharePoint Online での検索

SharePoint Online で検索する内容を検索するには、コンテンツをクロールして、検索インデックスに追加する必要があります。 コンテンツは、定義済みのクロールスケジュールに基づいて自動的にクロールされます (クロールスケジュールを変更することはできません)。 クローラーは、最後にクロールされて以降に変更が加えられたコンテンツを取得して、インデックスを更新します。 コンテンツがクロールされ、インデックスが更新されるようにするには、次の手順を実行します。

サイトコンテンツを検索可能にすることで、コンテンツを検出できることを確認します。 詳細については、「[サイトのコンテンツを検索可能にする](https://docs.microsoft.com/sharepoint/make-site-content-searchable)」を参照してください。

管理プロパティを変更した場合、またはクロールされたプロパティと管理プロパティのマッピングを変更した場合、変更が検索インデックスに反映されるようにするには、サイトを再クロールする必要があります。 

変更は検索スキーマで行われ、実際のサイトでは変更されないため、クローラーは自動的にサイトを再インデックス付けすることはありません。 

詳細については、「[サイト、ライブラリ、またはリストのクロールとインデックス再作成を手動で要求](https://docs.microsoft.com/sharepoint/crawl-site-conten)する」を参照してください。

 クロールと完全な再インデックスを手動で要求した後、少なくとも24時間待って、問題が発生しているかどうかを確認します。 

クロールを開始してから、フルインデックスを作成してから24時間以上経過した場合は、サポートケースをログに記録してください。 多くの場合、すでに解決策に取り組んでいます。 解決策を完成させるために少なくとも 24 時間を与えてください。

**重要**: サイト、ドキュメント (ライブラリ)、またはリストが削除されても検索結果に表示される場合は、アクセス試行時にエラー404ファイルが見つからないことをユーザーに通知する必要があります。 この問題は、詳細な調査のサポートケースとしてログに記録する必要があります。 



