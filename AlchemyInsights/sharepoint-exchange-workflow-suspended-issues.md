---
title: SharePoint Online の使用を開始する
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 285c580d69efb369fa6a60066165123e3c91b0a7
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051646"
---
# <a name="workflows-in-sharepoint"></a>SharePoint のワークフロー

SharePoint のワークフローでメールが送信されていない場合、組織が Exchange Online の送信者制限を行っている可能性があります。

次の項目のいずれかに該当する場合は、「ワークフローは中断されています」エラー メッセージが発生する可能性があります。

- SharePoint Online に、SharePoint 2010 または SharePoint 2013 ワークフロー プラットフォームの種類を使用しているワークフローがあります。

- ワークフローは、ユーザー設定のメール メッセージを一度に 200 を超えるユーザー、または 1 日に 1 万を超える受信者に送信するか、1 分あたり 30 件を超えるメッセージを送信するように、構成されています。

ワークフローを実行すると、電子メールメッセージは送信されず、[内部の状態] が "中断" または "受信者に送信できません" に設定されましたという内容のエラー メッセージが表示されます。

詳細については、次の[記事](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)を参照してください。

