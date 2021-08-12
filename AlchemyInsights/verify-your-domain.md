---
title: ドメインの検証
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 9e258cfc70c57fe787830d659dc52f4696768bea164d3be9ce7bcb9e7123c5a9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971020"
---
# <a name="verify-your-domain"></a>ドメインの検証

 **レコードがインターネット経由で更新されていない可能性があります。**
  
通常、ユーザーへの新しいレコードの表示には数分しかかかりませんが、場合によっては、数時間かかることもあります。 
  
- 既にその時間は待っている場合、DNS ホストで正確な値をコピーし、TXT 検証レコードに貼り付けたことを二重に確認してください。よくある原因の 1 つとして、レコードの「MS=」部分が含められていないことがあります。この部分も含める必要があります。

- DNS ホストによっては、インターネット全体で更新されるようにゾーン ファイル (DNS レコードが保存されているファイル) を保存するという作業も必要になります。Microsoft がレコードを表示し、確認できるように、変更内容は必ず保存してください。
