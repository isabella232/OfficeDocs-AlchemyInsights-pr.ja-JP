---
title: 外部グループを無効にする方法
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 09d8b134a4e99912301aa92c2e989fec9dd30a7b
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656392"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="cc213-102">外部グループを無効にする方法</span><span class="sxs-lookup"><span data-stu-id="cc213-102">How to disable External Groups</span></span>

<span data-ttu-id="cc213-p101">Exchange トランスポート ルール (ETRs)、一連の会社の情報が共有されているを防ぐために予防的な制御を適用する外部メッセージング Yammer。外部のグループを作成するユーザーを制限するために (ETR)、Exchange トランスポート ルールを構成し、Exchange のトランスポート ルールを使用して外部のメッセージングをブロックする Yammer を構成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="cc213-p101">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared. In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="cc213-105">Exchange Online 管理センターでルールを作成した後は、Yammer に適用する ETR を設定するのには次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="cc213-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="cc213-106">Yammer にログオンし、検証済みの管理者と**管理センターの Yammer**の、C に移動**ontent とセキュリティ\>のセキュリティ設定します**。</span><span class="sxs-lookup"><span data-stu-id="cc213-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="cc213-107">**外部メッセージ**を、[選択**Yammer に、Exchange オンライン Exchange トランスポート ルール (ETRs) を適用します**。</span><span class="sxs-lookup"><span data-stu-id="cc213-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="cc213-108">**[保存]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="cc213-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="cc213-109">詳細については、 [Exchange のトランスポート ルールを使用した Yammer ネットワークでメッセージを外部のコントロール](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc213-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  

