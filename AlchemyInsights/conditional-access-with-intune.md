---
title: Intune で条件付きのアクセス
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 59f1aefaeec3d655b2388b00e7d58a8c2338504b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29477400"
---
# <a name="conditional-access-with-intune"></a>Intune で条件付きのアクセス

Intune で**条件付きのアクセス**を使用するには、3 つの手順が必要です。 
  
- どのようなリソースが保護されていると、条件は満たす必要があるこれらのリソースにアクセスする必要がある**条件付きのアクセス ポリシー**を作成します。などのデバイスは、企業の電子メールにアクセスする前に準拠している必要があります。 
    
- デバイスは準拠と見なされる前に満たす必要のある設定を定義するための**コンプライアンス ・ ポリシー**を作成します。などのデバイスは、準拠と見なされる前に、少なくとも 6 桁の暗証番号 (pin) が必要です。 
    
- **コンプライアンス ・ ポリシー**と**アクセス ポリシーの条件**の両方が必要なユーザーのグループを対象としたことを確認します。Azure Active Directory 内の特定のユーザー グループを作成するこの必要があります。 
    
詳細情報
  
- [条件付きアクセスのベスト プラクティス](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/best-practices)
    
- [条件付きアクセスの概要](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

