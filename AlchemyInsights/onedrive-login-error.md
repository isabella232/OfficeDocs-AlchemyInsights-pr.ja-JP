---
title: One Drive ログイン エラー AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982624"
---
# <a name="onedrive-login-error-aadsts50011"></a>One Drive ログイン エラー AADSTS50011

OneDrive アプリにサインインしたときに、「AADSTS50011: 要求で指定された返信 URL が返信と一致しません」というエラーが表示された場合は、次のことを確認してください。

OneDrive のバージョンはバージョン 20.052.XXXX.XXXX 以上である必要があります。 バージョンを確認するには、通知領域で、青い OneDrive アイコンをクリックして、 **[ヘルプと設定]、[設定]、[バージョン情報]** の順に選択します。

ネットワークが **g.live.com** と **oneclient.sfx.ms** へのトラフィックをブロックする場合があります。 そのトラフィックがブロックされている場合、OneDrive は自動的に更新できません。 ネットワーク管理者と協力して、これらの URL にアクセスできるようにします。 [これらのエンドポイント](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide)は、Microsoft 365 プランを使用しているお客様にはアクセス可能である必要があります。

現在のバージョンの OneDrive を手動で取得する必要がある場合は、[https://aka.ms/getonedrive](https://aka.ms/getonedrive) を参照してください。
