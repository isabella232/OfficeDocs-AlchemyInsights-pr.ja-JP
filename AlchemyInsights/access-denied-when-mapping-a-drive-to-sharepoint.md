---
title: ドライブを SharePoint にマップしようとするとアクセスが拒否される
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: c41bfd9d25c8aa946a4ec5156be6d2424f4e2133
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/15/2019
ms.locfileid: "36737482"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a>ネットワーク ドライブにマップされた SharePoint ライブラリに関する問題を修正します

マップされたネットワーク ドライブを参照すると、次のいずれかのメッセージが表示されることがあります。
  
- **\\パスにアクセスできません。このネットワーク リソースを使用するアクセス許可がない可能性があります。アクセス許可があるかどうかを確認するには、このサーバーの管理者に問い合わせてください。**

- **アクセスが拒否されました。この場所のファイルを開く前に、まず Web サイトを信頼済みサイトのリストに追加し、Web サイトを参照して、自動的にログインするオプションを選択してください。**

[マップされたネットワーク ドライブのトラブルシューティングのヘルプを表示します](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)。
  
ライブラリをネットワーク ドライブとしてマップすることは一時的であり、Internet Explorer でのみサポートされています。その代わりに、[ファイル オンデマンド](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx)を含む[新しい OneDrive 同期クライアントを使用して SharePoint ファイルを同期](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx)します。OneDrive 内のすべてのファイルに、ローカル記憶域を使用することなくアクセスします。
  