---
title: メールが有効なパブリックフォルダーへのメール配信の問題を修正する
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
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525118"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>メールが有効なパブリックフォルダーへのメール配信の問題を修正する

外部の送信者がメッセージをメールが有効なパブリックフォルダーに送信できず、送信者がエラーを受信できなかった場合 **(550 5.4.1)**、パブリックフォルダーの電子メールドメインが、次のような内部の中継ドメインとして構成されていることを確認します。権限のあるドメイン:

1. [Exchange 管理センター (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center)を開きます。

2. [**メールフロー** \> **承認済みドメイン**] に移動して、承認済みドメインを選択し、[**編集**] をクリックします。

3. [プロパティ] ページが開いたら、ドメインの種類が [**権限**あり] に設定されている場合は、値を [**内部の中継**] に変更し、[**保存**] をクリックします。

外部の送信者がアクセス許可を持っていないエラーを受け取った場合 **(550 5.7.13)**、 [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)で次のコマンドを実行して、パブリックフォルダー内の匿名ユーザーのアクセス許可を確認します。

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`たとえば、 `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`のようになります。

外部ユーザーがこのパブリックフォルダーに電子メールを送信できるようにするには、CreateItems アクセス権をユーザー Anonymous に追加します。 たとえば、`Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` などです。
