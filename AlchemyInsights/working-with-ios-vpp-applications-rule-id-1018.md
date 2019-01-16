---
title: IOS アプリケーション ルール Id 1018 の VPP の操作
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 5bcfb6dd7222bd102ff2620c19bfb943e7bd9591
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28298209"
---
# <a name="working-with-ios-vpp-applications"></a>IOS VPP のアプリケーションを使用します。

機能、制約、および確認する手順について説明する[Microsoft Intune を使用してボリューム購入プログラムを通じて購入した場合、iOS アプリを管理する方法](https://docs.microsoft.com/intune/vpp-apps-ios)を参照して Apple ボリューム購入プログラムと Microsoft Intune でのサポートを使用します。 
  
 **の一般的な問題:**「IOS VPP アプリ、自分のユーザーに割り当てましたが、インストールに失敗しました」。 
  
- これは、複数のモバイル デバイス管理プロバイダー間で 1 つの VPP トークンを使用する場合に発生します。Apple 社の VPP のトークンは、1 つのプロバイダーでのみ使用できます。複数のプロバイダーと VPP のトークンを使用する場合は、Intune にトークンを再度アップロードする必要があります。
    
- インストールの合計数がライセンスの数を超える場合にも、インストールが失敗することができます。**Intune モバイル アプリケーション**には、ライセンスの使用状況レポートを表示するのには\>**アプリケーションのライセンス**のページです。使用中のライセンスを再利用する方法についてを参照してください[この記事](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)。
    

