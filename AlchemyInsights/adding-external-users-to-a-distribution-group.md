---
title: 外部ユーザーを配布グループに追加する場合
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 8/22/2017
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: ce0c589e1661fb4607452fe2e8f897758b2718e8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36494532"
---
# <a name="add-external-users-to-a-distribution-group"></a>外部ユーザーを配布グループに追加する場合

外部の連絡先を配布グループ (DG) に追加する作業は次の 2 段階プロセスになっています。
  
1. 外部ユーザーのメール連絡先を作成する:
    
    1. 管理センターで、[**ユーザー**]  >  [[連絡先](https://admin.microsoft.com/adminportal/home#/Contact)] ページに移動します。 
    
    2. [**連絡先を追加する**] を選択します。
    
    3. 連絡先の情報を入力し、[**保存**] を選択します。
    
2. メール連絡先を DG に追加する:
    
    1. 管理センターで、[**グループ**]  >  [[グループ](https://admin.microsoft.com/adminportal/home#/groups)] ページに移動します。 
    
    2. 外部ユーザーを追加する DG を見つけたらそれを選択し、編集ダイアログを開きます。
    
    3. [**メンバー**] タブで [**すべてのメンバーの表示と管理**] を選択します。  
    
    4. [**メンバーを追加する**] を選択します。
    
    5. 前の手順で作成したメール連絡先を選択し、[**保存**] を選択します。
    
これらの手順を実行した後に、外部ユーザーと DG の間でメールの送受信ができない場合は、内部ユーザーからのメールのみが許可されるように DG にマークされている可能性があります。 [こちら](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx)の指示に従ってこの構成の確認と修正を行えます。
  
 **注:** グループの種類が "配布グループ" ではなく "Office 365 グループ" の場合、これらの手順は適用されません。 その場合は、Outlook からグループに外部ユーザーを直接追加できます。 Office 365 グループ ゲストに関する詳細情報および外部ゲストを追加する手順については、[この記事](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)を参照してください。
  