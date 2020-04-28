---
title: 外部グループを無効にする方法
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720773"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="dbeea-102">外部グループを無効にする方法</span><span class="sxs-lookup"><span data-stu-id="dbeea-102">How to disable External Groups</span></span>

<span data-ttu-id="dbeea-p101">Yammer の外部メッセージングでは Exchange トランスポート ルール (ETR) を適用します。このルールは、会社情報が共有されないようにするプロアクティブ コントロールのセットです。ユーザーが外部グループを作成できないように、Exchange トランスポート ルール (ETR) を構成し、Exchange トランスポート ルールを使用して外部メッセージをブロックするように Yammer を構成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="dbeea-p101">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared. In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="dbeea-105">Exchange Online 管理センターでルールを作成したら、次の手順に従って、Yammer で適用されるように ETR を設定します。</span><span class="sxs-lookup"><span data-stu-id="dbeea-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="dbeea-106">認証管理者として Yammer にログインし、[**Yammer 管理センター**] から、**[コンテンツとセキュリティ] \> [セキュリティ設定**] の順に移動します。</span><span class="sxs-lookup"><span data-stu-id="dbeea-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="dbeea-107">**[外部メッセージング]** で、**[Exchange Online Exchange トランスポート ルール (ETR) を Yammer で適用する]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="dbeea-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="dbeea-108">**[保存]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="dbeea-108">Choose **Save**.</span></span>

<span data-ttu-id="dbeea-109">詳細については、「[Yammer ネットワーク内の外部メッセージングを無効にする](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dbeea-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  