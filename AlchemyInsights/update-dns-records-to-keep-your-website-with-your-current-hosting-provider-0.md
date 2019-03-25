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
ms.custom: ''
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: f2cdb319e56b82c09b7a9856c81a45e69dee6759
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/22/2019
ms.locfileid: "30760991"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>DNS レコードを更新して現在のホスティング プロバイダーに Web サイトを維持する

1. [ [ドメイン](https://portal.office.com/adminportal/home#/Domains) ] ページで、ドメインの一覧から、Web サイトで使用しているドメインを選択し、管理ウィンドウで [ **DNS 設定** ] を選択します。 
    
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
    

