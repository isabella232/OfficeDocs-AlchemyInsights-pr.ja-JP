---
title: メールボックスの監査を有効にする
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: bd94ec10f9df2e72ec6e3d8552d2eb80212a9d78
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29500287"
---
# <a name="enable-mailbox-auditing"></a>メールボックスの監査を有効にする

1 人のユーザーまたは組織全体のいずれかのメールボックスの監査を有効にするには、電源のリモート シェルから次のコマンドレットを実行してください。
  
 **1 人のユーザー**
  
セット-メールボックスの識別情報"Jane Dow"AuditEnabled $true
  
 **組織**
  
Get メールボックス ResultSize 無制限-{RecipientTypeDetails - eq「構成」} のフィルターを適用します。$True を設定メールボックス AuditEnabled
  
[詳細情報](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

