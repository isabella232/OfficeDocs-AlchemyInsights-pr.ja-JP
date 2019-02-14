---
title: プロファイルの同期
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: d1a72a85767e36fefbfa8eee266befcaf2e48af0
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "29920093"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>自分のプロファイルの変更は、SharePoint ユーザー プロファイル アプリケーションに同期されますか。

SharePoint Online では、Active Directory Import タイマー ジョブ (AD Import) を使用して、ユーザーとグループをユーザー プロファイル アプリケーションにインポートします。 
  
1. 変更は AD Import によって SharePoint Online のディレクトリ ストアからユーザー プロファイル アプリケーションに同期されます。これらの変更は一括で処理されます。
    
2. タイマー ジョブは、変更が同期されるまで実行されます。
    
> [!NOTE]
> ジョブの実行にかかる時間は処理する変更の数によって異なります。変更の数が多いと、時間も長くなります。サービス レベル アグリーメント (SLA) では、SharePoint Online ディレクトリでのユーザーに対する変更は 24 時間でユーザー プロファイル アプリケーションに反映されるものと規定されています。 
  
[SharePoint Online でのユーザープロファイルの同期に関する詳細情報](https://go.microsoft.com/fwlink/?linkid=875671)
  

