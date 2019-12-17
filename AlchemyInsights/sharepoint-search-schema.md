---
title: SharePoint Online で検索スキーマを管理する
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 9836cf139e97fc556995a8f0ad38c51c5c2392ac
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042968"
---
# <a name="manage-search-schema-in-sharepoint-online"></a>SharePoint Online で検索スキーマを管理する

検索スキーマでは、検索対象、検索方法、検索 Web サイトに検索結果を表示する方法を制御します。 

次の方法の詳細については、「[SharePoint Online で検索スキーマを管理する](https://docs.microsoft.com/sharepoint/manage-search-schema)」を参照してください。 
- 検索スキーマを変更する。
- 管理プロパティを作成する。
- クロールされたマップのクロールされたプロパティを管理プロパティにマップする。

検索スキーマの管理については、次の点にご注意ください。

- スキーマの変更を行うときに **アプリケーションが一時停止しています** という警告を受け取った場合、これはサービスの保守を行っている最中の一時的な状態に過ぎません。 

    24 時間以上経過しても警告が表示される場合は、サポート ケースを記録してください。
- 管理プロパティを変更するか、新しい管理プロパティを追加すると、その変更はコンテンツが再クロールされた後でのみ有効になります。 SharePoint Online では、定義されたクロール スケジュールに従って、クロールが自動的に行われます。
- 変更が確実にクロールされるよう、[リストやライブラリのインデックスの再作成を具体的に要求](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)することができます。 

検索スキーマの完全な概要については、「[Introducing Search Schema for SharePoint (SharePoint の検索スキーマの概要)](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)」を参照してください。 


