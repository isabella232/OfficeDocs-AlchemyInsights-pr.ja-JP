---
title: AllowSelfServicePurchase policy を設定または表示できません
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/16/2020
ms.locfileid: "42094398"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="3eecb-102">AllowSelfServicePurchase policy を設定または表示できません</span><span class="sxs-lookup"><span data-stu-id="3eecb-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="3eecb-103">AllowSelfServicePurchase policy を設定または表示しようとすると、次のエラーメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="3eecb-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="3eecb-104">*HandleError: PolicyId ' AllowSelfServicePurchase '、ErrorMessage-基になる接続が閉じられました。送信で予期しないエラーが発生しました。*</span><span class="sxs-lookup"><span data-stu-id="3eecb-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="3eecb-105">これは、以前のバージョンのトランスポート層セキュリティ (TLS) が原因である可能性があります。</span><span class="sxs-lookup"><span data-stu-id="3eecb-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="3eecb-106">MSCommerce サービスを接続するには、TLS 1.2 以上を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3eecb-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="3eecb-107">TLS プロトコルを有効または有効にするには、次の手順を実行してください。1.2、verify、および retry。</span><span class="sxs-lookup"><span data-stu-id="3eecb-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="3eecb-108">PowerShell コマンドプロンプト (PS C::\)次のコマンドを入力して、TLS プロトコルをバージョン1.2 に設定します。</span><span class="sxs-lookup"><span data-stu-id="3eecb-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    <span data-ttu-id="3eecb-109">\[Net.tcp Pointmanager]:: SecurityProtocol = \[Net.tcp protocol type]:: Tls12</span><span class="sxs-lookup"><span data-stu-id="3eecb-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span></span>

2. <span data-ttu-id="3eecb-110">次のコマンドを使用して、使用されている TLS プロトコルを確認します。</span><span class="sxs-lookup"><span data-stu-id="3eecb-110">Verify the TLS protocol(s) in use, with the following command:</span></span>

    <span data-ttu-id="3eecb-111">\[Net.tcp: ServicePointManager]:: SecurityProtocol</span><span class="sxs-lookup"><span data-stu-id="3eecb-111">\[Net.ServicePointManager]::SecurityProtocol</span></span> 

3. <span data-ttu-id="3eecb-112">必要に応じて、Get または Update コマンドを再試行します。</span><span class="sxs-lookup"><span data-stu-id="3eecb-112">Retry the Get or Update commands as needed.</span></span>

