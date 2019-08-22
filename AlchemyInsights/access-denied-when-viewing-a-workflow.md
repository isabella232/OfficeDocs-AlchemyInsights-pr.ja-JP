---
title: ワークフローを表示しようとするとアクセスが拒否される
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 53bd9285e49e220f880eea21923f261302003127
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495828"
---
# <a name="access-denied-when-viewing-a-workflow"></a>ワークフローを表示しようとするとアクセスが拒否される

SharePoint グループのメンバーシップがすべてのユーザーに設定されていないと、SharePoint グループにメールを送信する SharePoint 2013 ワークフローを表示しようとする際に「アクセスが拒否されました」というエラー メッセージが表示されることがあります。
  
 **この問題を解決するには、次の操作を行います。**
  
 1. すべてのユーザーに SharePoint グループのメンバーが表示されるようにします。
  
 2. メールの宛先または CC 行から SharePoint グループを削除します。
  
 3. SharePoint グループのメンバーシップの表示設定を変更できない場合は、To または CC 行にユーザーを明示的に追加します。
  
詳細を表示するには、 [/_vti_bin/client.svc/sp.utilities.utility.SendEmail に対する承認されていない HTTP](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)を参照してください。
  