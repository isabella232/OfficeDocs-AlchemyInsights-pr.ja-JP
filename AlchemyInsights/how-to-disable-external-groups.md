---
title: 外部グループを無効にする方法
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704133"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="da5c2-102">外部グループを無効にする方法</span><span class="sxs-lookup"><span data-stu-id="da5c2-102">How to disable External Groups</span></span>

<span data-ttu-id="da5c2-p101">Yammer の外部メッセージングでは Exchange トランスポート ルール (ETR) を適用します。このルールは、会社情報が共有されないようにするプロアクティブ コントロールのセットです。ユーザーが外部グループを作成できないように、Exchange トランスポート ルール (ETR) を構成し、Exchange トランスポート ルールを使用して外部メッセージをブロックするように Yammer を構成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="da5c2-p101">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared. In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="da5c2-105">Exchange Online 管理センターでルールを作成したら、次の手順に従って、Yammer で適用されるように ETR を設定します。</span><span class="sxs-lookup"><span data-stu-id="da5c2-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="da5c2-106">認証管理者として Yammer にログインし、[**Yammer 管理センター**] から、**[コンテンツとセキュリティ] \> [セキュリティ設定**] の順に移動します。</span><span class="sxs-lookup"><span data-stu-id="da5c2-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="da5c2-107">**[外部メッセージング]** で、**[Exchange Online Exchange トランスポート ルール (ETR) を Yammer で適用する]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="da5c2-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="da5c2-108">**[保存]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="da5c2-108">Choose **Save**.</span></span>

<span data-ttu-id="da5c2-109">詳細については、「[Yammer ネットワーク内の外部メッセージングを無効にする](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="da5c2-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  