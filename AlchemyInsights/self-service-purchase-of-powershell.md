---
title: PowerShell のセルフサービス購入
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: e6cc504ebef19cbe78f576d9b207fe2d951d0ef5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47739975"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="94a42-102">PowerShell のセルフサービス購入</span><span class="sxs-lookup"><span data-stu-id="94a42-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="94a42-103">MSCommerce PowerShell モジュールを使用するには、TLS 1.2 を備えた Windows 10 デバイスにインストールする必要があります (ローカル管理者の許可が必要です)。</span><span class="sxs-lookup"><span data-stu-id="94a42-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="94a42-104">MSCommerce モジュールをインポートして接続します。</span><span class="sxs-lookup"><span data-stu-id="94a42-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="94a42-105">ログインするように求められたら、グローバルまたは請求管理者の役割の資格情報を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="94a42-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="94a42-106">TLS 1.2 がない場合、ポリシーを取得または更新しようとすると、次のエラーが表示される場合があります。</span><span class="sxs-lookup"><span data-stu-id="94a42-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="94a42-107">*ErrorMessage - 基になる接続が閉じられました: 送信で予期しないエラーが発生しました*。</span><span class="sxs-lookup"><span data-stu-id="94a42-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



