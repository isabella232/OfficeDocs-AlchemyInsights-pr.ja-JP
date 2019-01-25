---
title: プロファイルの同期
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a32cf9e623d1be7a2c85ef4951c6eb7f001b7db0
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29477436"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>SharePoint ユーザー プロファイル アプリケーションを自分のプロファイルの変更内容の同期と

SharePoint Online は、ユーザー プロファイル アプリケーションにユーザーとグループをインポートするのには Active Directory のインポートのタイマー ジョブ (AD のインポート) を使用します。 
  
1. AD のインポートでは、SharePoint のオンライン ディレクトリ ストアからユーザー プロファイル アプリケーションへの変更を同期します。これらの変更は、バッチで処理されます。
    
2. 変更が同期されるまで、タイマー ジョブが実行されます。
    
> [!NOTE]
> ジョブの実行にかかる時間は、変更を処理するための数によって異なります。多数の変更に時間がかかります。サービス レベル契約 (SLA) では、SharePoint のオンライン ディレクトリ内のユーザーへの変更を 24 時間でのユーザー プロファイル アプリケーションに反映されることを示しています。 
  
[SharePoint Online でユーザー プロファイルの同期に関する詳細情報](https://go.microsoft.com/fwlink/?linkid=875671)
  

