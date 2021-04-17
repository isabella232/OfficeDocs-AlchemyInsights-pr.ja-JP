---
title: 電子情報開示のエクスポート用に Chromium ブラウザー ベースの Microsoft Edge を使用する
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3473"
- "3100022"
ms.openlocfilehash: 7ee724e5109effce8883be50e360948313c84b34
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834376"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a><span data-ttu-id="a2d40-102">電子情報開示のエクスポート用に Chromium ブラウザー ベースの Microsoft Edge を使用する</span><span class="sxs-lookup"><span data-stu-id="a2d40-102">Using Microsoft Edge based on Chromium browsers for Ediscovery export</span></span>

<span data-ttu-id="a2d40-103">最近行われた変更により、Microsoft Edge ブラウザーでは、ClickOnce のサポートが既定では有効化されないようになりました。</span><span class="sxs-lookup"><span data-stu-id="a2d40-103">Due to a recent change, Microsoft Edge browsers will no longer have ClickOnce support enabled by default.</span></span> <span data-ttu-id="a2d40-104">Microsoft 365 電子情報開示エクスポート ツールを継続して使用するには、Microsoft Internet Explorer を使用するか、Microsoft Edge での ClickOnce のサポートを有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="a2d40-104">To continue using the Microsoft 365 eDiscovery Export Tool, you will either need to use Microsoft Internet Explorer or enable ClickOnce Support in Microsoft Edge.</span></span> 

<span data-ttu-id="a2d40-105">Chromium に基づく Microsoft Edge で ClickOnce のサポートを有効にするには、次の操作を行います。</span><span class="sxs-lookup"><span data-stu-id="a2d40-105">To enable ClickOnce Support in Microsoft Edge based on Chromium:</span></span> 
1. <span data-ttu-id="a2d40-106">Microsoft Edge ブラウザーで、edge://flags/#edge-click-once にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="a2d40-106">In your Microsoft Edge browser, visit edge://flags/#edge-click-once.</span></span>
2. <span data-ttu-id="a2d40-107">[ClickOnce Support] オプションで、値を [**Default (規定)**] または [**Disabled (無効)**] から [**Enabled (有効)**] に変更します。</span><span class="sxs-lookup"><span data-stu-id="a2d40-107">For the ClickOnce Support option, change the value from **Default** or **Disabled** to **Enabled**.</span></span> 
3. <span data-ttu-id="a2d40-p102">ブラウザー ウィンドウの下部で、[**Restart (リスタート)**] を選択します。 </span><span class="sxs-lookup"><span data-stu-id="a2d40-p102">At the bottom of the browser window, select **Restart**. </span></span><br>
 <span data-ttu-id="a2d40-109">Microsoft Edge を再起動すると、変更が有効になります。</span><span class="sxs-lookup"><span data-stu-id="a2d40-109">The change will take effect after restarting Microsoft Edge.</span></span> 

<span data-ttu-id="a2d40-110">この手順およびエクスポート ツールをインストールする手順の詳細については、「[コンテンツ検索の結果をエクスポートする](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2d40-110">For information on this and steps for installing the  export tool, see: [ Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>