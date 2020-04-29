---
title: ワークフローを表示しようとするとアクセスが拒否される
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687335"
---
# <a name="access-denied-when-viewing-a-workflow"></a>ワークフローを表示しようとするとアクセスが拒否される

SharePoint グループのメンバーシップがすべてのユーザーに設定されていないと、SharePoint グループにメールを送信する SharePoint 2013 ワークフローを表示しようとする際に「アクセスが拒否されました」というエラー メッセージが表示されることがあります。
  
 **この問題を解決するには、次の操作を行います。**
  
 1. すべてのユーザーに SharePoint グループのメンバーが表示されるようにします。
  
 2. メールの宛先または CC 行から SharePoint グループを削除します。
  
 3. SharePoint グループのメンバーシップの表示設定を変更できない場合は、To または CC 行にユーザーを明示的に追加します。
  
詳細については「[/_vti_bin/client.svc/sp.utilities.utility.SendEmail への HTTP 権限エラー](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)」を参照してください。
  