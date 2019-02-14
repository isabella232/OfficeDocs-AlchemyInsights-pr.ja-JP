---
title: UPN 同期が無効
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 983796ce8fb7e8b52c0ce31aa13597b53cc9e038
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "29921713"
---
# <a name="upn-sync-disabled"></a>UPN 同期が無効

2016 年 3 月 30 日より前に Azure AD との同期を開始した場合は、次の Azure AD PowerShell コマンドレットを実行して、ご自分の組織に対してのみ UPN あいまい一致を有効にします。
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
UPN あいまい一致は、2016 年 3 月 30 日以降に Azure AD との同期を開始した組織に対しては自動的に有効になります。
  
UPN やその他の同期機能であいまい一致を有効にする方法の詳細については、「[Azure AD Connect 同期サービスの機能](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)」を参照してください。
  

