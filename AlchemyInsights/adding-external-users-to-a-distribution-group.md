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
ms.openlocfilehash: ce67797a1838630ab3a42e1eeeefc401a0e3f753
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906881"
---
# <a name="adding-external-users-to-a-distribution-group"></a>外部ユーザーを配布グループに追加する場合

外部の連絡先を配布グループ (DG) に追加する作業は次の 2 段階プロセスになっています。
  
1. 外部ユーザーのメール連絡先を作成する:
    
1. [ここ](https://admin.microsoft.com/adminportal/home#/Contact)をクリックし、管理ポータルの連絡先編集ページに移動します。 
    
2. [**連絡先の追加**] をクリックします。
    
3. 連絡先の情報を入力し、[**保存**] をクリックします。
    
2. メール連絡先を DG に追加する:
    
1. [ここ](https://admin.microsoft.com/adminportal/home#/groups)をクリックし、グループ ページに移動します。 
    
2. 外部ユーザーを追加する DG を見つけたらそれをクリックし、編集ダイアログを開きます。
    
3. [**メンバー**] 一覧の [**編集**] ボタンをクリックします。 
    
4. [**メンバーの追加**] をクリックします。
    
5. 前の手順で作成したメール連絡先を選択し、[**保存**] をクリックします。
    
以上の手順に従っても外部ユーザーが DG にメールを送信できないか、DG からメールを受信できない場合、内部ユーザーからのメールのみがその DG に許可されている可能性があります。[こちら](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx)の操作方法に従うことでこの構成を確認し、修正できます。
  
 **注:** グループの種類が "配布グループ" ではなく "Office 365 グループ" の場合、これらの操作方法は適用されません。その場合、外部ユーザーは Outlook または Outlook on the web からグループに直接追加できます。O365 グループ ゲストに関する詳しい説明と外部ゲストの追加方法については、[こちらの記事](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)でご確認いただけます。
  

