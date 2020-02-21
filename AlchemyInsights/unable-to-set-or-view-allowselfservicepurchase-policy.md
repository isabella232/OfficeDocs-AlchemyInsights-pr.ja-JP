---
title: AllowSelfServicePurchase ポリシーを設定または表示できません
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
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/16/2020
ms.locfileid: "42094398"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="fac95-102">AllowSelfServicePurchase ポリシーを設定または表示できません</span><span class="sxs-lookup"><span data-stu-id="fac95-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="fac95-103">AllowSelfServicePurchase ポリシーを設定または表示しようとすると、次のエラー メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="fac95-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="fac95-104">*HandleError: PolicyId 'AllowSelfServicePurchase' で製品ポリシーを取得できませんでした、ErrorMessage - 基になる接続が閉じられました: 送信で予期しないエラーが発生しました。*</span><span class="sxs-lookup"><span data-stu-id="fac95-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="fac95-105">これは、トランスポート層セキュリティ (TLS) の古いバージョンが原因である可能性があります。</span><span class="sxs-lookup"><span data-stu-id="fac95-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="fac95-106">MSCommerce サービスに接続するには、TLS 1.2 以降を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="fac95-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="fac95-107">次の手順を試して、TLS プロトコルを 1.2 に有効化/設定し、確認して、再試行します。</span><span class="sxs-lookup"><span data-stu-id="fac95-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="fac95-108">PowerShell コマンドプロンプトで (PS C:\) 次のコマンドを入力して、TLS プロトコルをバージョン 1.2 に設定します。</span><span class="sxs-lookup"><span data-stu-id="fac95-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    <span data-ttu-id="fac95-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span><span class="sxs-lookup"><span data-stu-id="fac95-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span></span>

2. <span data-ttu-id="fac95-110">次のコマンドを使用して、使用中の TLS プロトコルを確認します。</span><span class="sxs-lookup"><span data-stu-id="fac95-110">Verify the TLS protocol(s) in use, with the following command:</span></span>

    <span data-ttu-id="fac95-111">\[Net.ServicePointManager]::SecurityProtocol</span><span class="sxs-lookup"><span data-stu-id="fac95-111">\[Net.ServicePointManager]::SecurityProtocol</span></span> 

3. <span data-ttu-id="fac95-112">必要に応じて、Get または Update コマンドを再試行します。</span><span class="sxs-lookup"><span data-stu-id="fac95-112">Retry the Get or Update commands as needed.</span></span>

