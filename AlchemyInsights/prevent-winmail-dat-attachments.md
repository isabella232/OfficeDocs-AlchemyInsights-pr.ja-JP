---
title: 2589 組織からのメール メッセージに Winmail.dat 添付ファイルが含まれないようにする
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2589
ms.assetid: ''
ms.openlocfilehash: 41ab3f22499994cda5883834ff54e5767c69265b
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36397239"
---
# <a name="help-prevent-winmaildat-attachments-in-email-messages-from-your-organization"></a><span data-ttu-id="3a30e-102">組織からのメール メッセージに Winmail.dat 添付ファイルが含まれないようにする</span><span class="sxs-lookup"><span data-stu-id="3a30e-102">Help prevent Winmail.dat attachments in email messages from your organization</span></span>

<span data-ttu-id="3a30e-103">管理者として、次の手順を試します。</span><span class="sxs-lookup"><span data-stu-id="3a30e-103">As an admin, try these steps:</span></span>

1. <span data-ttu-id="3a30e-104">[[Exchange 管理センター](https://outlook.office365.com/ecp/)] を開きます。</span><span class="sxs-lookup"><span data-stu-id="3a30e-104">Open the [Exchange admin center](https://outlook.office365.com/ecp/)</span></span>

2. <span data-ttu-id="3a30e-105">[**メール フロー**]  >  [**リモート ドメイン**] の順に移動します。</span><span class="sxs-lookup"><span data-stu-id="3a30e-105">Go to **Mail flow** > **Remote domains**.</span></span>

3. <span data-ttu-id="3a30e-106">**Default** という既定のリモート ドメインを選択し、[**編集**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="3a30e-106">Select the default remote domain named **Default**, and then click **Edit**.</span></span>

4. <span data-ttu-id="3a30e-107">[**リッチテキスト形式の使用**] セクションで、 [**行なわない**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3a30e-107">In the **Use Rich-text format** section, select **Never**.</span></span>

<span data-ttu-id="3a30e-108">詳細については、「[リモート ドメインのメッセージ形式を指定する](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3a30e-108">For more information, see [Specify the message format for remote domains](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format).</span></span>
