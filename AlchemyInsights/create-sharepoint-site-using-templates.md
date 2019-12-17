---
title: SharePoint Online のサイトを作成する
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 458990889d3c074820527982cbfa6e2d198d3e66
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052474"
---
# <a name="create-sharepoint-sites-using-templates"></a>テンプレートを使用して SharePoint サイトを作成する

SharePoint サイト テンプレートは、特定のビジネス ニーズに基づいて設計された作成済みの定義です。 詳細については、「[テンプレートを使用して、さまざまな種類の SharePoint サイトを作成する](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)」を参照してください。

これは、SharePoint Online でサイトまたはリストをテンプレートとして保存することに関する一般的な問題 / 解決策です。 

**[テンプレートとしてサイト/リストを保存] ボタンが利用できないか、見つからない**

管理者は、テンプレート機能を有効にするためにカスタム スクリプトを許可する必要があります。 詳細な手順、例、および考慮事項については、次を参照してください。 

- [カスタム スクリプトを許可または禁止する](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- [テンプレートとしてサイトを保存] コマンドはサポートされていないため、SharePoint Server 発行インフラストラクチャを使用するサイトで問題が発生する可能性があります。

**サイト テンプレートを作成できない、またはサイト テンプレートが正常に機能しない**

テンプレートに[機能](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx)が設定されていないため、有効になりません。 現在のサイト コレクションで機能を有効にできない場合は、サイト テンプレートを使用してサイトを作成することはできません。

- サイト テンプレートの作成がブロックされる可能性があるため、リストまたはライブラリが[リスト ビューのしきい値](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59)の5000項目を超えていないかどうかを確認します。

- サイトが多すぎるリソースを使用している可能性があり、サイト テンプレートが50 MB の制限を超えています。


- ルックアップ列を使用するリストのデータを表示する際に問題が発生します。 詳細については、「[SharePoint Online で、テンプレートから作成したリストに正しいルックアップ リスト データが表示されない](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)」を参照してください。

共通の問題と解決策の詳細については、 「[サイト テンプレートを作成して使用する](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)」を参照してください。



