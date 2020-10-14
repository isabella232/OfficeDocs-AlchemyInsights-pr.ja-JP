---
title: UPN 同期が無効
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749519"
---
# <a name="upn-sync-disabled"></a>UPN 同期が無効

2016 年 3 月 30 日より前に Azure AD との同期を開始した場合は、次の Azure AD PowerShell コマンドレットを実行して、ご自分の組織に対してのみ UPN あいまい一致を有効にします。
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
UPN あいまい一致は、2016 年 3 月 30 日以降に Azure AD との同期を開始した組織に対しては自動的に有効になります。
  
UPN やその他の同期機能であいまい一致を有効にする方法の詳細については、「[Azure AD Connect 同期サービスの機能](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)」を参照してください。
  

