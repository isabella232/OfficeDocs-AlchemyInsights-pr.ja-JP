---
title: 2491テナントまたはユーザーの上書きにより配信された "フィッシングからの電子メールメッセージの通知" ポリシー
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36397240"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>[テナントまたはユーザーの上書きによって配信されたフィッシング] ポリシーから電子メールメッセージを通知する

「テナントまたはユーザーの上書きによって配信されたフィッシング」という名前の既定の通知ポリシーが、Office 365 ATP P1 および P2 ライセンスを使用してテナントにロールアウトされています。 この通知を受信した場合は、次の手順を使用して調査する必要があります。

1. 通知メッセージで、[**警告の表示**] をクリックして、セキュリティ & コンプライアンスセンターの [**通知**] ページに移動します。

2. 通知を選択して、エクスプローラーで**メッセージリストを表示**したり、**メッセージを表示**したりするオプションを表示します。 どちらのオプションでも、メッセージの ID が含まれているメッセージの詳細が表示されます。 脅威エクスプローラーのリンクによって、通知の条件に一致するメッセージが自動的にフィルター処理されることに注意してください。 脅威エクスプローラーで日付フィルターを調整する必要がある場合があります。

手動で構成された上書きが原因で、フィッシングメッセージが配信されました。

- 許可された送信者またはドメインがユーザーによって設定されている。

- スパム対策ポリシーで、管理者によって設定された送信者またはドメインの許可。

- 接続フィルターポリシーで許可されている IP アドレス。

- でメッセージを許可するように構成されたメールフロールール (トランスポートルールとも呼ばれます)。

メッセージが誤ってフィッシングとしてマークされていると思われる場合は、Outlook[レポートメッセージアドイン](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2)を使用して、メッセージサンプルを Microsoft に送信します。
