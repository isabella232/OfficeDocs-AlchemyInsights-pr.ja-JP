---
title: メールが有効なパブリック フォルダーへの電子メール配信の問題を修正する
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: f7b5e5a230d26870d5e95e8762b5874f73723c6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525118"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>メールが有効なパブリック フォルダーへの電子メール配信の問題を修正する

外部の送信者が、メールが有効なパブリック フォルダーにメッセージを送信できないときに、送信者に **見つかりませんでした (550 5.4.1)** というエラーが示される場合は、そのパブリック フォルダーの電子メール ドメインが、権限のあるドメインではなく、内部の中継ドメインとして構成されていることを確認してください。

1. [Exchange 管理センター (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center) を開きます。

2. **[メール フロー]** \> **[承認済みドメイン]** に移動して、承認済みドメインを選択してから **[編集]** をクリックします。

3. プロパティ ページが表示されます。このページで、ドメインの種類が **[権限あり]** に設定されている場合は、その値を **[内部の中継]** に変更してから **[保存]** をクリックします。

外部送信者に **アクセス許可がありません (550 5.7.13)** というエラーが示される場合は、[Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) で次のコマンドを実行して、パブリック フォルダーの匿名ユーザーに対するアクセス許可を確認してください: 

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`。たとえば、`Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` のようにします。

このパブリック フォルダーに外部ユーザーが電子メールを送信できるようにするには、ユーザー Anonymous に CreateItems アクセス権限を追加します。 たとえば、`Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` のようにします。
