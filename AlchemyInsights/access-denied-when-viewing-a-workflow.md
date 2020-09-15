---
title: ワークフローを表示しようとするとアクセスが拒否される
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688807"
---
# <a name="access-denied-when-viewing-a-workflow"></a>ワークフローを表示しようとするとアクセスが拒否される

SharePoint グループのメンバーシップがすべてのユーザーに設定されていないと、SharePoint グループにメールを送信する SharePoint 2013 ワークフローを表示しようとする際に「アクセスが拒否されました」というエラー メッセージが表示されることがあります。
  
 **この問題を解決するには、次の操作を行います。**
  
 1. すべてのユーザーに SharePoint グループのメンバーが表示されるようにします。
  
 2. メールの宛先または CC 行から SharePoint グループを削除します。
  
 3. SharePoint グループのメンバーシップの表示設定を変更できない場合は、To または CC 行にユーザーを明示的に追加します。
  
詳細については「[/_vti_bin/client.svc/sp.utilities.utility.SendEmail への HTTP 権限エラー](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)」を参照してください。
  