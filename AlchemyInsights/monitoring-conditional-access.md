---
title: 条件付きアクセスの監視
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 06307b57475e8828e6d4e5e01625d5100576f12b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29476573"
---
# <a name="monitoring-conditional-access"></a>条件付きアクセスの監視

条件付きアクセスの対象となるユーザー組織のアクセス要件を満たしていない場合は、メールによる通知が表示されます。を解決するのには、次の解決策の 1 つ以上お勧めします。
  
- デバイスが登録すると見なされます場合は、会社のポータル アプリケーションに移動し、企業ポータルに表示されたことを確認するユーザーを案内します。しない場合、ユーザーがデバイスを登録する必要があります。
    
- Azure ポータルに移動**Intune\>デバイス対応**です。**モニター** ] の下には、**準拠のデバイス**をクリックします。ユーザーのデバイスに準拠としてマークされていることを確認するのには、デバイスのコンプライアンス レポートを表示します。 
    
- Azure ポータルに移動**Intune\>デバイス対応**です。[**管理**] で [**ポリシー**] をクリックします。コンプライアンス ・ ポリシーの一覧で、プロファイルが、ユーザーのデバイスに割り当てられていることを確認します。プロファイルが割り当てられていない場合 Intune はデバイスのコンプライアンスのステータスを確認できません。 
    
- ユーザーの条件付きアクセスの割り当てを編集します。
    
1. Azure ポータルに移動**Intune\>条件付きアクセス\>ポリシー**
    
2. リストからポリシーを選択します。
    
3. [**ユーザーとグループ**
    
4. 他のユーザーに特定のポリシーをターゲットに**含める**] ボックスの一覧に追加します。ポリシーから人が省略されていることを確認するには、**除外**リストに追加します。 
    
参照:[デバイスの条件付きのアクセスを監視する方法](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)
  

