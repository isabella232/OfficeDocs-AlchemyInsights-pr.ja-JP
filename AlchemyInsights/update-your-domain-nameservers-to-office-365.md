---
title: Microsoft を指すようにドメインネームサーバーを更新する
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: b49ca9422f582f906fc6c108c85cc26150474548
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719998"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a>Microsoft を指すようにドメインネームサーバーを更新する

注: ネーム サーバーの変更は、反映されるまで最大 48 時間かかる場合があります。
  
Microsoft を使用してドメインをセットアップするには、レジストラーのネームサーバーを更新する必要があります。ドメインレジストラーでネームサーバーレコードを作成または編集します。
  
1. ご利用のドメイン レジストラーの Web サイトにアクセスして、ネーム サーバーを編集できる領域を見つけます。

2. 以下の値に一致する 2 つのネーム サーバー レコードを作成または編集します。

  - ns1.bdm.microsoftonline.com

  - ns2.bdm.microsoftonline.com

3. 変更を保存します。

この記事の詳細な手順については、「[ネームサーバーを変更して、Microsoft 365 を任意のドメインレジストラーでセットアップする](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)」を参照してください。
  