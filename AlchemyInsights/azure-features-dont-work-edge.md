---
title: Microsoft Edge で Azure 機能が正常に機能しない場合の対処方法
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8315"
- "9004429"
ms.openlocfilehash: 710489bd7dcb10f5c953c83e87bdad030c47cfda7dbd38e1eceae78bfe0d8790
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "57345760"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Microsoft Edge で Azure 機能が正常に機能しない場合の対処方法

Microsoft Edge には、セキュリティ ゾーンに関連する既知の問題があり、Azure ユーザーが Windows Admin Center にログインする方法に影響を与える可能性があります。 詳細については、「[Edge での既知の問題](https://go.microsoft.com/fwlink/?linkid=2140608)」を参照してください。 Microsoft Edge で Azure 機能を使用する際に問題が発生した場合は、次の手順を試してください。

1. スタート メニューの **[検索]** バーで、「**インターネット オプション**」と入力し、それを選択します。
1. **[インターネット プロパティ]** で、**[セキュリティ]** タブを選択します。
1. **[信頼済みサイト]** を選び、**[サイト]** を選びます。
1. ゲートウェイ URL、<https://login.microsoftonline.com>、および <https://login.live.com> を追加し、**[閉じる]** を選択します。
1. **[インターネット プロパティ]** で、**[プライバシー]** タブを選択します。
1. [ポップアップ ブロック] セクションで、**[設定]** を選択します。 ゲートウェイ URL、<https://login.microsoftonline.com>、および <https://login.live.com> を追加してから、**[閉じる]** を選択します。