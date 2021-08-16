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
ms.openlocfilehash: 933f977a09b013778799e0dc0c40c2959824cfbe6aa766495f7d1e1aab242878
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54097563"
---
# <a name="multiple-active-sessions-to-the-same-mailbox"></a>同じメールボックスへの複数のアクティブなセッション

Exchange リソースの使用をコントロールするために、メールボックスには "予算" があります。

予算超過の例外は、次の状況によってトリガーされますが、これに限定されません：

- 同じ Outlook Web App セッション内でいくつかのブラウザーのタブが開かれます。　　

- 同じメールボックスへのいくつかのアクティブな　Outlook Web App　セッション。

- 他のいくつかのクライアントアプリケーション (Outlook、Outlook Mobile、サードパーティのクライアントアプリ) は、同時にメールボックスにアクセスします。　　　

- 検索要求の実行など、長時間実行される操作は、別のアクティブなメールボックスセッションから実行されます。

