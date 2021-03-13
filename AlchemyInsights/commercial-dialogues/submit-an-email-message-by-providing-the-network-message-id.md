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
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751233"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="7b9c3-102">ネットワーク メッセージ ID を指定して電子メール メッセージを送信する</span><span class="sxs-lookup"><span data-stu-id="7b9c3-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="7b9c3-103">[**新規送信**] フライアウトで、[**メール** と **ネットワーク メッセージ ID**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7b9c3-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="7b9c3-104">Outlook の電子メール メッセージにてメッセージ ID を検索するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="7b9c3-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="7b9c3-105">電子メール メッセージをダブルクリックして開きます。</span><span class="sxs-lookup"><span data-stu-id="7b9c3-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="7b9c3-106">[**ファイル**]  >  [**プロパティ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7b9c3-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="7b9c3-107">メモ帳または空白の Word 文書を開き、[**インターネット ヘッダー**] ボックスにあるコンテンツをコピーして、開いている文書に貼り付けて、見やすくします。</span><span class="sxs-lookup"><span data-stu-id="7b9c3-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="7b9c3-108">[**X-MS-Exchange-Organization-Network-Message-ID**] フィールドを指定します。</span><span class="sxs-lookup"><span data-stu-id="7b9c3-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="7b9c3-109">**後の値:** は、送信に必要な ID です。</span><span class="sxs-lookup"><span data-stu-id="7b9c3-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="7b9c3-110">[**受信者**] で、このメールのすべての受信者の迷惑メール フォルダーにメールが届く場合は、[**すべて選択**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7b9c3-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="7b9c3-111">表示されない場合は、問題を報告したユーザーのみを選択します。</span><span class="sxs-lookup"><span data-stu-id="7b9c3-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="7b9c3-112">[**送信の理由**] で [**ブロックが必要**] を選択した場合は、メッセージを [**迷惑メール**]、[**フィッシング詐欺**]、または [**マルウェア**] としてブロックするかどうかを指定し、[**送信**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7b9c3-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="7b9c3-113">詳細については、「[疑いのあるスパム、フィッシング、URL、ファイルをスキャンのために Microsoft に送信する方法](https://go.microsoft.com/fwlink/?linkid=2101479)」 を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7b9c3-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
