---
title: SharePoint Online の使用を開始する
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: afb1ef115d364ee3e2cf09ea850adb57ad1d44e6
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "35085928"
---
# <a name="workflows-in-sharepoint"></a>SharePoint のワークフロー

SharePoint のワークフローがメールを送信していない場合は、組織で Exchange Online の送信者制限が発生している可能性があります。

次の項目のいずれかに該当する場合は、「ワークフローは中断されています」エラー メッセージが発生する可能性があります。

- SharePoint Online に、SharePoint 2010 または SharePoint 2013 ワークフロー プラットフォームの種類を使用しているワークフローがあります。

- ワークフローは、ユーザー設定のメール メッセージを一度に 200 を超えるユーザー、または 1 日に 1 万を超える受信者に送信するか、1 分あたり 30 件を超えるメッセージを送信するように、構成されています。

ワークフローを実行すると、電子メールメッセージは送信されず、[内部の状態] が "中断" または "受信者に送信できません" に設定されましたという内容のエラー メッセージが表示されます。

詳細については、次の[記事](https://support.office.com/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US)を参照してください。

