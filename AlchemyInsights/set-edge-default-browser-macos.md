---
title: Mac OS デバイスの既定ブラウザとして Microsoft Edge を設定する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: e04f8931ef12c426a5c3d5f617fc5f5d5c3a15c6fe43f7b84a7e97e8ee04e3fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54073965"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a>Mac OS デバイスの既定ブラウザとして Microsoft Edge を設定する

次の 2 つの方法のいずれかを使用して、Microsof tEdge を既定のブラウザーとして設定します。

方法 1 : Microsoft Edge が既に既定のブラウザーとして設定されている macOS のイメージでデバイスをフラッシュします。

方法 2 : DefaultBrowserSettingEnabled ポリシーを設定して、Microsoft Edge を既定のブラウザーとして設定するようにユーザーに促します。

どちらの方法でも、ユーザーは既定のブラウザを変更できます。 このため、メソッド 1 を使用した場合でも、DefaultBrowserSettingEnabled ポリシーを展開することをお勧めします。 ポリシーの展開後にユーザーが既定のブラウザーを変更すると、ポリシーにより、既定のブラウザーを Microsoft Edge に戻すようにユーザーに求められます。
