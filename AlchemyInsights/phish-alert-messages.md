---
title: "\"テナントまたはユーザーの上書きによって配信されたフィッシング\" ポリシーからのアラート メール メッセージ 2491"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728616"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>"テナントまたはユーザーの上書きによって配信されたフィッシング" ポリシーからのアラート メール メッセージ 

"テナントまたはユーザーの上書きによって配信されたフィッシング" という名前の既定のアラート ポリシーは、Office 365 ATP P1 および P2 ライセンスのテナントに展開されています。 このアラートを受け取った場合は、次の手順に従って調査してください。

1. アラート メッセージで、[**アラートの表示**] をクリックし、セキュリティ/コンプライアンス センターの [**アラート**] ページに移動します。

2. アラートを選択し、[**メッセージ リストの表示**] または [**エクスプローラーでメッセージを表示**] を行うためのオプションを表示させます。 いずれのオプションの場合でも、メッセージ ID などのメッセージの詳細情報が表示されます。 [脅威エクスプローラー] リンクでは、アラートの条件に一致するメッセージが自動的にフィルター処理されます。 脅威エクスプローラーで日付フィルターの調整が必要になる場合があります。

手動で構成された上書きにより、フィッシング メッセージが送信されました:

- ユーザーによって設定された、許可された送信者またはドメイン。

- 迷惑メール対策ポリシーの管理者によって設定された、許可された送信者またはドメイン。

- 接続フィルター ポリシーで許可されている IP アドレス。

- メッセージの受信を許可するように構成されたメール フロー ルール (トランスポート ルールとも呼ばれます)。

メッセージが誤ってフィッシングとしてマークされていると思われる場合は、Outlook の[迷惑メール報告アドイン](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2)を使用してメッセージのサンプルを Microsoft に送信してください。
