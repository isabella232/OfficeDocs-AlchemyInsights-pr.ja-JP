---
title: 外部ユーザーを配布グループに追加する
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737878"
---
# <a name="add-external-users-to-a-distribution-group"></a>外部ユーザーを配布グループに追加する

外部連絡先を配布グループ (DG) に追加するには、2段階の手順を実行します。
  
1. 外部ユーザーのメール連絡先を作成する:
    
    1. 管理センターで、[**ユーザー** > の[連絡先](https://admin.microsoft.com/adminportal/home#/Contact)] ページに移動します。 
    
    2. [**連絡先の追加**] を選択します。
    
    3. 連絡先の情報を入力し、[**追加**] を選択します。
    
2. メール連絡先を DG に追加する:
    
    1. 管理センターで、[**グループ** > [グループ](https://admin.microsoft.com/adminportal/home#/groups)] ページに移動します。 
    
    2. 外部ユーザーの追加先となる DG を見つけ、それを選択して [編集] ダイアログを開きます。
    
    3. [**メンバー** ] タブで、[**すべて表示**] を選択し、メンバーを管理します。 
    
    4. [**メンバーの追加**] を選択します。
    
    5. 前の手順で作成したメール連絡先を選択し、[**保存**] を選択します。
    
これらの手順を実行した後、外部ユーザーがメールを DG に送信できない、またはメールを受信できない場合は、DG が内部ユーザーからの電子メールのみを許可するように設定されている可能性があります。 この構成を確認して、[ここに記載](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)されている手順に従って修正することができます。
  
 **注:** これらの手順は、グループの種類が "配布グループ" ではなく "Office 365 group" である場合には適用されません。 その場合は、Outlook から直接グループに外部ユーザーを追加することができます。 Office 365 グループゲストの詳細と、外部ゲストの追加手順については、[この記事](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)を参照してください。
  