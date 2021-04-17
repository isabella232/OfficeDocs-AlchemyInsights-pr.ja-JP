---
title: AllowSelfServicePurchase ポリシーを設定または表示できません
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
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826096"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="e51b6-102">AllowSelfServicePurchase ポリシーを設定または表示できません</span><span class="sxs-lookup"><span data-stu-id="e51b6-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="e51b6-103">AllowSelfServicePurchase ポリシーを設定または表示しようとすると、次のエラー メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="e51b6-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="e51b6-104">*HandleError: PolicyId 'AllowSelfServicePurchase' で製品ポリシーを取得できませんでした、ErrorMessage - 基になる接続が閉じられました: 送信で予期しないエラーが発生しました。*</span><span class="sxs-lookup"><span data-stu-id="e51b6-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="e51b6-105">これは、トランスポート層セキュリティ (TLS) の古いバージョンが原因である可能性があります。</span><span class="sxs-lookup"><span data-stu-id="e51b6-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="e51b6-106">MSCommerce サービスに接続するには、TLS 1.2 以降を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e51b6-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="e51b6-107">次の手順を試して、TLS プロトコルを 1.2 に有効化/設定し、確認して、再試行します。</span><span class="sxs-lookup"><span data-stu-id="e51b6-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="e51b6-108">PowerShell コマンドプロンプトで (PS C:\) 次のコマンドを入力して、TLS プロトコルをバージョン 1.2 に設定します。</span><span class="sxs-lookup"><span data-stu-id="e51b6-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="e51b6-109">次のコマンドを使用して、使用中の TLS プロトコルを確認します。</span><span class="sxs-lookup"><span data-stu-id="e51b6-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="e51b6-110">必要に応じて、Get または Update コマンドを再試行します。</span><span class="sxs-lookup"><span data-stu-id="e51b6-110">Retry the Get or Update commands as needed.</span></span>

