---
title: SharePoint Online のサイトを作成する
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 7c24a0cf3bcae0f2780c1cb33c911cb38c1ca5cb
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36515003"
---
# <a name="create-sharepoint-sites-using-templates"></a>テンプレートを使用して SharePoint サイトを作成する

SharePoint サイト テンプレートは、特定のビジネス ニーズに基づいて設計された作成済みの定義です。 詳細については、「[テンプレートを使用して、さまざまな種類の SharePoint サイトを作成する](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)」を参照してください。

ここでは、サイトまたはリストを Sharepoint Online でテンプレートとして保存する場合の一般的な問題と解決策を示します。 

**[サイトの保存/リストテンプレート] ボタンが使用できない、または見つからない**

管理者は、テンプレート機能を有効にするためにカスタム スクリプトを許可する必要があります。 詳細な手順については、「例」と「考慮事項」をご覧ください。 

- [カスタム スクリプトを許可または禁止する](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- [テンプレートとしてサイトを保存] コマンドはサポートされていないため、SharePoint Server 発行インフラストラクチャを使用するサイトで問題が発生する可能性があります。

**サイト テンプレートを作成できないか、正しく機能しない**

テンプレートが[機能](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx)を持たず、アクティブ化されない場合があります。 現在のサイト コレクションで機能を有効にできない場合は、サイト テンプレートを使用してサイトを作成することはできません。

- サイト テンプレートの作成がブロックされる可能性があるため、リストまたはライブラリが[リスト ビューのしきい値](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59)の5000項目を超えていないかどうかを確認します。

- サイトで使用されているリソースが多すぎるため、サイトテンプレートが 50 MB の制限を超えている可能性があります。


- ルックアップ列を使用するリストのデータを表示する際に問題が発生します。 詳細については、「[テンプレートで生成されるリスト」で、SharePoint Online の適切な参照リストからのデータを表示しません](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a)。

一般的な問題と解決策の詳細については、「[サイトテンプレートを作成して使用する](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)」を参照してください。



