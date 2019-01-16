---
title: UPN の同期が無効になっています。
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: d00f10688ec775c22d60a9089e291c265ada46f1
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28298259"
---
# <a name="upn-sync-disabled"></a>UPN の同期が無効になっています。

2016 年 3 月 30 日前に AD を Azure に同期を開始する場合は、UPN ソフト一致する組織のみを有効にするのには、次の Azure AD の PowerShell コマンドレットを実行します。
  
 **セット-MsolDirSyncFeature-EnableSoftMatchOnUpn をフィーチャー-$True を有効にします。**
  
ソフト一致の UPN が自動的に有効に 2016 年 3 月 30 日以降に、Azure AD への同期を開始する組織です。
  
ソフト一致 UPN およびその他の同期機能を有効にする方法については、 [Azure AD 接続の同期サービスの機能](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)を参照してください。
  

