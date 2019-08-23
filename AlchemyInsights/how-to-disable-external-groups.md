---
title: 外部グループを無効にする方法
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4683a71438ec31f9e9211404a9c66c4e45e0e1df
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36540906"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="27559-102">外部グループを無効にする方法</span><span class="sxs-lookup"><span data-stu-id="27559-102">How to disable External Groups</span></span>

<span data-ttu-id="27559-p101">Yammer の外部メッセージングでは Exchange トランスポート ルール (ETR) を適用します。このルールは、会社情報が共有されないようにするプロアクティブ コントロールのセットです。ユーザーが外部グループを作成できないように、Exchange トランスポート ルール (ETR) を構成し、Exchange トランスポート ルールを使用して外部メッセージをブロックするように Yammer を構成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="27559-p101">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared. In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="27559-105">Exchange Online 管理センターでルールを作成したら、次の手順に従って、Yammer で適用されるように ETR を設定します。</span><span class="sxs-lookup"><span data-stu-id="27559-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="27559-106">確認済み管理者として Yammer にログオンし、 **yammer 管理センター**で [C の**コンテンツとセキュリティ\>の設定**] に移動します。</span><span class="sxs-lookup"><span data-stu-id="27559-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="27559-107">**[外部メッセージング]** で、**[Exchange Online Exchange トランスポート ルール (ETR) を Yammer で適用する]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="27559-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="27559-108">[**保存**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="27559-108">Choose **Save**.</span></span>

<span data-ttu-id="27559-109">詳細については、[Exchange トランスポート ルールを使用した Yammer ネットワークでの外部メッセージングの制御](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="27559-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  