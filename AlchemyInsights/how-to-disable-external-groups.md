---
title: 外部グループを無効にする方法
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4d911c319c3e8e327f9b3af3ba67816e646bc468
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "29899141"
---
# <a name="how-to-disable-external-groups"></a>外部グループを無効にする方法

Yammer の外部メッセージングでは Exchange トランスポート ルール (ETR) を適用します。このルールは、会社情報が共有されないようにするプロアクティブ コントロールのセットです。ユーザーが外部グループを作成できないように、Exchange トランスポート ルール (ETR) を構成し、Exchange トランスポート ルールを使用して外部メッセージをブロックするように Yammer を構成する必要があります。 
  
Exchange Online 管理センターでルールを作成したら、次の手順に従って、Yammer で適用されるように ETR を設定します。
  
- 認証管理者として Yammer にログオンして、**Yammer 管理センター**で **[コンテンツとセキュリティ]、[セキュリティ設定]** の順に移動します。
    
- **[外部メッセージング]** で、**[Exchange Online Exchange トランスポート ルール (ETR) を Yammer で適用する]** を選択します。
    
- [**保存**] を選択します。 
    
詳細については、[Exchange トランスポート ルールを使用した Yammer ネットワークでの外部メッセージングの制御](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)に関するページを参照してください。
  

