---
title: 2589 組織からのメール メッセージに Winmail.dat 添付ファイルが含まれないようにする
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2589
ms.assetid: ''
ms.openlocfilehash: f67c4146af419a590651c8e0673fd59fabd7eae7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47693740"
---
# <a name="help-prevent-winmaildat-attachments-in-email-messages-from-your-organization"></a><span data-ttu-id="b1878-102">組織からのメール メッセージに Winmail.dat 添付ファイルが含まれないようにする</span><span class="sxs-lookup"><span data-stu-id="b1878-102">Help prevent Winmail.dat attachments in email messages from your organization</span></span>

<span data-ttu-id="b1878-103">管理者として、次の手順を試します。</span><span class="sxs-lookup"><span data-stu-id="b1878-103">As an admin, try these steps:</span></span>

1. <span data-ttu-id="b1878-104">[[Exchange 管理センター](https://outlook.office365.com/ecp/)] を開きます。</span><span class="sxs-lookup"><span data-stu-id="b1878-104">Open the [Exchange admin center](https://outlook.office365.com/ecp/).</span></span>

2. <span data-ttu-id="b1878-105">[**メール フロー**]  >  [**リモート ドメイン**] の順に移動します。</span><span class="sxs-lookup"><span data-stu-id="b1878-105">Go to **Mail flow** > **Remote domains**.</span></span>

3. <span data-ttu-id="b1878-106">**Default** という既定のリモート ドメインを選択し、[**編集**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="b1878-106">Select the default remote domain named **Default**, and then click **Edit**.</span></span>

4. <span data-ttu-id="b1878-107">[**リッチテキスト形式の使用**] セクションで、 [**行なわない**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="b1878-107">In the **Use Rich-text format** section, select **Never**.</span></span>

<span data-ttu-id="b1878-108">詳細については、「[リモート ドメインのメッセージ形式を指定する](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b1878-108">For more information, see [Specify the message format for remote domains](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format).</span></span>
