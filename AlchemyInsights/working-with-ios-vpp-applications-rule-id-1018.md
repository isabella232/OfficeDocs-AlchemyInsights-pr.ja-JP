---
title: iOS VPP アプリケーション ルール ID 1018 との連携
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 65b9a727171a7551068717f6327f15e1aa8e6bed
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "29917501"
---
# <a name="working-with-ios-vpp-applications"></a>iOS VPP アプリケーションとの連携

Apple Volume Purchase Program の機能、制約、利用するための手順、および Microsoft Intune でのサポートについては、「[Volume Purchase Program で購入した iOS アプリを Microsoft Intune で管理する方法](https://docs.microsoft.com/intune/vpp-apps-ios)」を参照してください。 
  
 **一般的な問題:** "iOS VPP アプリをユーザーに割り当てましたが、インストールに失敗しました。" 
  
- これは、複数のモバイル デバイス管理プロバイダーとの間で 1 つの VPP トークンを使用している場合に発生することがあります。Apple からの VPP トークンは 1 つのプロバイダーでのみ使用できます。複数のプロバイダーで VPP トークンを使用した場合、そのトークンを Intune に再アップロードする必要があります。
    
- また、インストールの合計回数がライセンスの数を超えた場合にも、インストールが失敗することがあります。ご利用のライセンスの利用状況レポートを表示するには、**Intune Mobile アプリ**、[**アプリ ライセンス**] ページの順に移動します。使用中のライセンスを再使用する方法については、[この記事](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)を参照してください。
    

