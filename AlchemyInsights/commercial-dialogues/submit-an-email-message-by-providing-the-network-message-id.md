---
title: ネットワーク メッセージ ID を指定して電子メール メッセージを送信する
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1a6f9815a36cc267a815ff9757d713afed5d95aec4f7c537135c88cadf26cc51
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929922"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a>ネットワーク メッセージ ID を指定して電子メール メッセージを送信する

1. [**新規送信**] フライアウトで、[**メール** と **ネットワーク メッセージ ID**] を選択します。
2. Outlook の電子メール メッセージにてメッセージ ID を検索するには、次の手順を実行します。
    1. 電子メール メッセージをダブルクリックして開きます。
    1. [**ファイル**]  >  [**プロパティ**] を選択します。
    1. メモ帳または空白の Word 文書を開き、[**インターネット ヘッダー**] ボックスにあるコンテンツをコピーして、開いている文書に貼り付けて、見やすくします。
    1. [**X-MS-Exchange-Organization-Network-Message-ID**] フィールドを指定します。 **後の値:** は、送信に必要な ID です。
3. [**受信者**] で、このメールのすべての受信者の迷惑メール フォルダーにメールが届く場合は、[**すべて選択**] を選択します。 表示されない場合は、問題を報告したユーザーのみを選択します。
4. [**送信の理由**] で [**ブロックが必要**] を選択した場合は、メッセージを [**迷惑メール**]、[**フィッシング詐欺**]、または [**マルウェア**] としてブロックするかどうかを指定し、[**送信**] を選択します。

詳細については、「[疑いのあるスパム、フィッシング、URL、ファイルをスキャンのために Microsoft に送信する方法](https://go.microsoft.com/fwlink/?linkid=2101479)」 を参照してください。
