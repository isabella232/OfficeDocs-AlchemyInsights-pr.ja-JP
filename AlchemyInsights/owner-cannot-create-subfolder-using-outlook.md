---
title: 所有者は Outlook を使用してサブフォルダーを作成できない
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665723"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>所有者は Outlook を使用してサブフォルダーを作成できない

**パブリック フォルダーの所有者が Outlook を使用してサブフォルダーを作成する場合、継続的な問題があります。この問題は間もなく修正されます。**

その間、次のいずれかの回避策を使用します。

1. 問題はデスクトップ ウィンドウ (すべてのバージョン) の Outlook にのみ影響するため、Outlook for MAC を使用してサブフォルダーを作成します。
2. EXO シェルまたは EAC を使用してサブフォルダーを作成するように管理者に指示する
3. ユーザーの DefaultPublicFolderMailbox/EffectivePublicFolderMailbox を、問題の原因となっているフォルダーのコンテンツ メールボックス以外のメールボックスに変更します。  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. 1 時間待って、Outlook クライアントを再起動します