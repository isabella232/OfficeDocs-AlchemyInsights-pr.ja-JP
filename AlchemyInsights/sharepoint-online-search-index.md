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
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "35174468"
---
# <a name="search-in-sharepoint-online"></a>SharePoint Online での検索

ユーザーが SharePoint Online のコンテンツを検索できるようにするには、コンテンツをクロールし、検索インデックスに追加する必要があります。 コンテンツは、事前に定義されたクロール スケジュールに基づいて自動的にクロールされます (クロール スケジュールは変更できません)。 クローラーは、最後にクロールを実行したとき以降に変更されたコンテンツを取得し、インデックスを更新します。 コンテンツがクロールされ、インデックスが更新されるようにするには、次の手順を実行します。

コンテンツを見つけることができるよう、サイト コンテンツを検索可能にします。 詳細については、「[サイトのコンテンツを検索可能にする](https://docs.microsoft.com/sharepoint/make-site-content-searchable)」を参照してください。

管理プロパティを変更した場合や、クロールされたプロパティと管理プロパティのマッピングを変更した場合は、サイトを再クロールしないと、検索インデックスに変更内容が反映されません。 

変更は検索スキーマ内で行われ、実際のサイトに対しては行われていないため、クローラーでサイトのインデックスが自動的に再作成されることはありません。 

詳細については、「[サイトのクロールとインデックス再作成を手動で要求する](https://docs.microsoft.com/sharepoint/crawl-site-conten)」を参照してください。

 手動によるクロールとインデックスの完全な再作成の要求後少なくとも 24 時間以上待ってから、問題が引き続き発生するかどうかを確認します。 

クロールとインデックスの完全な再作成の開始後 24 時間以上経過している場合は、サポート ケースを記録してください。 多くの場合、すでに解決策に取り組んでいます。 解決策を完成させるために少なくとも 24 時間を与えてください。

**重要**: サイト、ドキュメント (ライブラリ)、またはリストを削除した後も検索結果に表示される場合、ユーザーがアクセスを試みると [エラー 404 ファイルが見つかりません] というエラーが表示されるはずです。 この問題は、詳細な調査のためにサポート ケースとして記録する必要があります。 



