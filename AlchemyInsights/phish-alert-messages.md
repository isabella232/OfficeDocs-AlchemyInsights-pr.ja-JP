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
ms.openlocfilehash: 90b078147bbb1e60cba0a2de6e49a862469f93aa
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316363"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>"テナントまたはユーザーの上書きによって配信されたフィッシング" ポリシーからのアラート メール メッセージ 

Microsoft Defender for Office 365 P1 および P2 ライセンスを使用している組織では、"**テナントまたはユーザーの上書きによって配信されたフィッシング**" という名前の既定のアラート ポリシーを使用できます。 このアラートを受け取った場合は、次の手順に従って調査してください。

1. アラート メッセージで、[**アラートの表示**] をクリックし、Microsoft 365 Defender ポータルの [**アラート**] ページに移動します。

2. アラートを選択し、[**メッセージ リストの表示**] または [**エクスプローラーでメッセージを表示**] を行うためのオプションを表示させます。 いずれのオプションの場合でも、メッセージ ID などのメッセージの詳細情報が表示されます。 [脅威エクスプローラー] リンクでは、アラートの条件に一致するメッセージが自動的にフィルター処理されます。 脅威エクスプローラーで日付フィルターの調整が必要になる場合があります。

手動で構成された上書きにより、フィッシング メッセージが送信されました:

- ユーザーによって設定された、許可された送信者またはドメイン。
- 迷惑メール対策ポリシーの管理者によって設定された、許可された送信者またはドメイン。
- 接続フィルター ポリシーで許可されている IP アドレス。
- メッセージの受信を許可するように構成されたメール フロー ルール (トランスポート ルールとも呼ばれます)。

メッセージが誤ってフィッシングとしてマークされたと思われる場合は、[管理者報告](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)を使用してメッセージを Microsoft に報告してください。

ユーザーは、Outlook の[レポート メッセージ アドインまたはレポート フィッシング アドイン](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in)を使用して、メッセージ サンプルを Microsoft に送信できます。
