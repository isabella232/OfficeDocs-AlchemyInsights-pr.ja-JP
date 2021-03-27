---
title: 手動で Microsoft Edge にサインインする
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
- "8332"
- "9004625"
ms.openlocfilehash: f380d09dc14788205638cdee6aebe0b084ecab2f
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398662"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>手動で Microsoft Edge にサインインする

最初の実行エクスペリエンス時にユーザーが自動的にサインインしなかった場合、ユーザーはブラウザーの設定または ID ポップアップから手動でサインインできます。 サインインを管理するには、次のポリシーを使用します。

1. [NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) - ユーザーが常に Microsoft Edge で作業プロファイルを持つようにします。
2. [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) - 一連の信頼できるアカウントにサインインを制限します。
3. [BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) - サインインを無効にするか、ユーザーに強制的にサインインさせます。

