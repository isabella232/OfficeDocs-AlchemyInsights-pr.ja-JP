---
title: 条件付きアクセスを監視する
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "29902356"
---
# <a name="monitoring-conditional-access"></a>条件付きアクセスを監視する

条件付きアクセスで対象となるユーザーは、組織のアクセス要件を満たしていない場合には通知電子メールを受信します。この状態を解消するには、以下の 1 つ以上の解決策をお勧めします。
  
- そのデバイスが登録されていると推測される場合、ポータル サイト アプリに移動して、ポータル サイトに表示されていることを確認するようユーザーに勧めます。表示されない場合、ユーザーはそのデバイスを登録する必要があります。
    
- Azure Portal で **[Intune] \> [デバイスのポリシー準拠]** と移動します。**[モニター]** で **[デバイスのポリシー準拠]** をクリックします。デバイスのポリシー準拠レポートを表示して、ユーザーのデバイスがポリシー準拠と示されているかどうか確認します。 
    
- Azure Portal で **[Intune] \> [デバイスのポリシー準拠]** と移動します。**[管理]** で **[ポリシー]** をクリックします。ポリシー準拠ポリシーの一覧で、ユーザーのデバイスにプロファイルが割り当てられていることを確認します。プロファイルが割り当てられていない場合、Intune はデバイスのポリシー準拠状態を確認できません。 
    
- ユーザーの条件付きアクセス割り当てを編集します。
    
1. Azure Portal で、**[Intune] \> [条件付きアクセス] \> [ポリシー]** と移動します。
    
2. 一覧からポリシーを選択します。
    
3. **[ユーザーとグループ]** をクリックします。
    
4. 特定のユーザーに対して特定のポリシーを対象とするには、**[必要]** リストに追加します。対象ポリシーから特定のユーザーを除外するには、**[必要なし]** リストに追加します。 
    
参照資料: [条件付きアクセス デバイスを監視する方法](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

