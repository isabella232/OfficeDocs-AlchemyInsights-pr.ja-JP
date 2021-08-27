---
title: 126 OWA で「メールボックスが見つかりませんでした」というエラーが表示される場合
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 4938b889461f85ad32eae125151c2cc94879cd8b
ms.sourcegitcommit: 02562a6796d58991c7238ec81053c23633b3f823
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/25/2021
ms.locfileid: "58522359"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Outlook on the web で「メールボックスが見つかりませんでした」というエラーが表示される場合

Outlook Web App (OWA) エラーが発生した場合: "*ユーザー* のメールボックスが見つかりませんでした。" というエラーは、ログインしているユーザーに Exchange Onlince ライセンスと sp がないことを意味します。このユーザー アカウントに Exchange Online メールボックスは関連付けられません。 

組織の管理者は次の手順に従って Microsoft 365 管理センターから Exchange ライセンスをユーザーに割り当てることができます。

1. [[アクティブなユーザー]](https://portal.office.com/adminportal/home#/users) に移動し、ユーザーを選択してから **[製品ライセンス]**  >  **[編集]** の順に選択します。 
1. 要求された場所を設定する
1. Exchange Online サービス プランがあるライセンスを割り当てます。