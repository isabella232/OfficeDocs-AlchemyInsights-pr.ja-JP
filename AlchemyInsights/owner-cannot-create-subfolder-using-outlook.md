---
title: 所有者は Outlook を使用してサブフォルダーを作成できない
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836140"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>所有者は Outlook を使用してサブフォルダーを作成できない

**パブリック フォルダーの所有者が Outlook を使用してサブフォルダーを作成する場合、継続的な問題があります。この問題は間もなく修正されます。**

その間、次のいずれかの回避策を使用します。

1. 問題はデスクトップ ウィンドウ (すべてのバージョン) の Outlook にのみ影響するため、Outlook for MAC を使用してサブフォルダーを作成します。
2. EXO シェルまたは EAC を使用してサブフォルダーを作成するように管理者に指示する
3. ユーザーの DefaultPublicFolderMailbox/EffectivePublicFolderMailbox を、問題の原因となっているフォルダーのコンテンツ メールボックス以外のメールボックスに変更します。  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. 1 時間待って、Outlook クライアントを再起動します