---
title: SharePoint の検索結果にコンテンツが表示されない
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ffb6bf349f9e8c2323186a8fc3183325d1d7e1bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36517036"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>SharePoint の検索結果にコンテンツが表示されない

想定されるコンテンツが検索結果に表示されない場合は、次のトラブルシューティング手順を実行します。
  
1. 想定されるコンテンツを含む**サイト**が、検索結果にコンテンツを表示するように設定されていることを確認します。「[検索結果でサイトにコンテンツを表示する](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)」の手順を実行します。

2. 想定されるコンテンツを含む**リスト**または**ライブラリ**が、検索結果にコンテンツを表示するように設定されていることを確認します。「[検索結果にリストまたはライブラリのコンテンツを表示する](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)」の手順を実行します。

3. ページ、ドキュメント、またはカスタム ページ レイアウトが**メジャー バージョン**として公開されていることを確認します。「[SharePoint Online で検索がすべての結果を返さない](https://go.microsoft.com/fwlink/?linkid=874525)」の手順 3 を実行します。

4. ユーザーがコンテンツを表示するための**アクセス許可**を持っていることを確認します。「[SharePoint でのアクセス許可レベルについて](https://docs.microsoft.com/sharepoint/understanding-permission-levels)」の手順を実行します。
    
5. 新しい管理プロパティを追加して検索スキーマを変更した場合、管理プロパティを編集した場合、または管理プロパティを削除した場合は、クロールを要求し、インデックスの再作成が必要になります。 [サイト、ライブラリ、またはリストのクロールとインデックス再作成を手動で要求](https://docs.microsoft.com/sharepoint/crawl-site-content)する手順に従って、コンテンツの**インデックスを再**作成します。 この処理には時間がかかることがあります。24時間待ってから結果を再度確認してください。

詳細については、「[サイトのコンテンツを検索](https://docs.microsoft.com/sharepoint/make-site-content-searchable)可能にする」を参照してください。 
  
