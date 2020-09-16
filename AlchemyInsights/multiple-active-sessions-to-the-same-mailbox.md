---
title: 同じメールボックスへの複数のアクティブなセッション
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1836"
- "9000248"
ms.openlocfilehash: f4ae5c5afef9972ad4ffe74144d702ed58b2f437
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769728"
---
# <a name="multiple-active-sessions-to-the-same-mailbox"></a>同じメールボックスへの複数のアクティブなセッション

Exchange リソースの使用をコントロールするために、メールボックスには "予算" があります。

予算超過の例外は、次の状況によってトリガーされますが、これに限定されません：

- 同じ Outlook Web App セッション内でいくつかのブラウザーのタブが開かれます。　　

- 同じメールボックスへのいくつかのアクティブな　Outlook Web App　セッション。

- 他のいくつかのクライアントアプリケーション (Outlook、Outlook Mobile、サードパーティのクライアントアプリ) は、同時にメールボックスにアクセスします。　　　

- 検索要求の実行など、長時間実行される操作は、別のアクティブなメールボックスセッションから実行されます。

