---
title: Microsoft を指すようにドメイン ネームサーバーを更新する
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734916"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a>Microsoft を指すようにドメイン ネームサーバーを更新する

注: ネーム サーバーの変更は、反映されるまで最大 48 時間かかる場合があります。
  
Microsoft でドメインを設定するには、レジストラーのネーム サーバーを更新する必要があります。ドメイン レジストラーでネーム サーバー レコードを作成または編集します。
  
1. ご利用のドメイン レジストラーの Web サイトにアクセスして、ネーム サーバーを編集できる領域を見つけます。

2. 以下の値に一致する 2 つのネーム サーバー レコードを作成または編集します。

  - ns1.bdm.microsoftonline.com

  - ns2.bdm.microsoftonline.com

3. 変更を保存します。

詳細な手順については、「[任意のドメイン レジストラーで Microsoft 365 をセットアップするためにネームサーバーを変更する](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)」も参照してください。
  