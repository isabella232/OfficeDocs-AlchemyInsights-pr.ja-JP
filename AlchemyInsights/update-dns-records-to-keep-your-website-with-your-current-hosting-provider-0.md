---
title: DNS レコードを更新して現在のホスティング プロバイダーに Web サイトを維持する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a1ea0589def4945da64c73d68b2e4a3d64d6b83d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506412"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>DNS レコードを更新して現在のホスティング プロバイダーに Web サイトを維持する

1. [[ドメイン](https://portal.office.com/adminportal/home#/Domains)] ページの [ドメイン] リストで、web サイトで使用しているドメインを選択します。

2. [**+ 新しいカスタム レコード**] を選択し、次を入力します。

  - [ **DNS の種類** ] には、「 **A (アドレス)** 」と入力します。

  - [ **ホスト名またはエイリアス** ] には、「 **@** 」と入力します。

  - [ **IP アドレス** ] には、Web サイトが現在ホストされている場所の静的 IP アドレス (たとえば、172.16.140.1) を入力します。

    これは、Web サイトの *動的*  IP アドレスではなく、  *静的*  IP アドレスでなければなりません。 Web サイトがホストされているサイトで、一般向け Web サイトの静的 IP アドレスを取得できることを確認します。

3. [**保存**] を選択します。

さらに、CNAME レコードを作成して、Web サイトを顧客が簡単に見つけることができるようにすることもできます。
  
1. [ **+ 新しいカスタム レコード** ] を選択し、次の項目を入力します。

  - [ **DNS の種類** ] には、「 **CNAME (エイリアス)** 」と入力します。

  - [ **ホスト名またはエイリアス** ] には、「 **www** 」と入力します。

  - [ **ポイント先のアドレス** ] には、Web サイトの完全修飾ドメイン名 (FQDN) を入力します (例: contoso.com)。

2. [**保存**] を選択します。
