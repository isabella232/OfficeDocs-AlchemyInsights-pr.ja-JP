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
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29477193"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="0247e-102">IOS VPP のアプリケーションを使用します。</span><span class="sxs-lookup"><span data-stu-id="0247e-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="0247e-103">機能、制約、および確認する手順について説明する[Microsoft Intune を使用してボリューム購入プログラムを通じて購入した場合、iOS アプリを管理する方法](https://docs.microsoft.com/intune/vpp-apps-ios)を参照して Apple ボリューム購入プログラムと Microsoft Intune でのサポートを使用します。</span><span class="sxs-lookup"><span data-stu-id="0247e-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="0247e-104">**の一般的な問題:**「IOS VPP アプリ、自分のユーザーに割り当てましたが、インストールに失敗しました」。</span><span class="sxs-lookup"><span data-stu-id="0247e-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="0247e-p101">これは、複数のモバイル デバイス管理プロバイダー間で 1 つの VPP トークンを使用する場合に発生します。Apple 社の VPP のトークンは、1 つのプロバイダーでのみ使用できます。複数のプロバイダーと VPP のトークンを使用する場合は、Intune にトークンを再度アップロードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="0247e-p101">This can happen if a single VPP token is used across multiple mobile device management providers. VPP tokens from Apple may only be used with one provider. If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="0247e-p102">インストールの合計数がライセンスの数を超える場合にも、インストールが失敗することができます。**Intune モバイル アプリケーション**には、ライセンスの使用状況レポートを表示するのには\>**アプリケーションのライセンス**のページです。使用中のライセンスを再利用する方法についてを参照してください[この記事](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)。</span><span class="sxs-lookup"><span data-stu-id="0247e-p102">The installation can also fail if the total number of installations exceed the number of licenses. To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page. To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

