---
title: DNS レコードを更新して現在のホスティング プロバイダーに Web サイトを維持する
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: f868ce25d68f61da30d2db4de88aa83675c97857b3c1371cf2039e0b03895a64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007687"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>DNS レコードを更新して現在のホスティング プロバイダーに Web サイトを維持する

1. Microsoft 365 管理センターで **[セットアップ]**] > [[ドメイン]](https://admin.microsoft.com/Adminportal#/Domains) ページの順に移動し、ドメインのリストで、Web サイトに使用するドメインを選択します。

2. [ **+ 新しいカスタム レコード** ] を選択し、次の項目を入力します。

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
