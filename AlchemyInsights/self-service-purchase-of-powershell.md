---
title: PowerShell のセルフサービス購入
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
- "9001212"
- "3516"
ms.openlocfilehash: 48b5b0a1be1bc03d45a531a1093f18a3f750c37d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51797726"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="c7a78-102">PowerShell のセルフサービス購入</span><span class="sxs-lookup"><span data-stu-id="c7a78-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="c7a78-103">MSCommerce PowerShell モジュールを使用するには、TLS 1.2 を備えた Windows 10 デバイスにインストールする必要があります (ローカル管理者の許可が必要です)。</span><span class="sxs-lookup"><span data-stu-id="c7a78-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="c7a78-104">MSCommerce モジュールをインポートして接続します。</span><span class="sxs-lookup"><span data-stu-id="c7a78-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="c7a78-105">ログインするように求められたら、グローバルまたは請求管理者の役割の資格情報を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c7a78-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="c7a78-106">TLS 1.2 がない場合、ポリシーを取得または更新しようとすると、次のエラーが表示される場合があります。</span><span class="sxs-lookup"><span data-stu-id="c7a78-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="c7a78-107">*ErrorMessage - 基になる接続が閉じられました: 送信で予期しないエラーが発生しました*。</span><span class="sxs-lookup"><span data-stu-id="c7a78-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



