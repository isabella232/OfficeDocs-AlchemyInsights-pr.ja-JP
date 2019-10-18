---
title: iOS VPP アプリケーション ルール ID 1018 との連携
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: a0bbc1f49f251ef4f16300c8cca98e219008d17e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558006"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="b8724-102">iOS VPP アプリケーションとの連携</span><span class="sxs-lookup"><span data-stu-id="b8724-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="b8724-103">Apple Volume Purchase Program の機能、制約、利用するための手順、および Microsoft Intune でのサポートについては、「[Volume Purchase Program で購入した iOS アプリを Microsoft Intune で管理する方法](https://docs.microsoft.com/intune/vpp-apps-ios)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b8724-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="b8724-104">**一般的な問題:** "iOS VPP アプリをユーザーに割り当てましたが、インストールに失敗しました。"</span><span class="sxs-lookup"><span data-stu-id="b8724-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="b8724-p101">これは、複数のモバイル デバイス管理プロバイダーとの間で 1 つの VPP トークンを使用している場合に発生することがあります。Apple からの VPP トークンは 1 つのプロバイダーでのみ使用できます。複数のプロバイダーで VPP トークンを使用した場合、そのトークンを Intune に再アップロードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="b8724-p101">This can happen if a single VPP token is used across multiple mobile device management providers. VPP tokens from Apple may only be used with one provider. If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="b8724-p102">また、インストールの合計回数がライセンスの数を超えた場合にも、インストールが失敗することがあります。ご利用のライセンスの利用状況レポートを表示するには、**Intune Mobile アプリ**、[**アプリ ライセンス**] ページの順に移動します。使用中のライセンスを再使用する方法については、[この記事](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b8724-p102">The installation can also fail if the total number of installations exceed the number of licenses. To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page. To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
