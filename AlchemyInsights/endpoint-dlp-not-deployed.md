---
title: エンドポイント DLP がユーザーのデバイスに展開されていません
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/27/2021
ms.locfileid: "52732078"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a><span data-ttu-id="e4693-102">エンドポイント DLP がユーザーのデバイスに展開されていません</span><span class="sxs-lookup"><span data-stu-id="e4693-102">Endpoint DLP not deployed to user's device</span></span>

<span data-ttu-id="e4693-103">エンドポイント データ損失防止 (DLP) 設定がユーザーのデバイスに適用されていない場合は、次の要件を満たしていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="e4693-103">If the Endpoint data loss prevention (DLP) setting has not applied to a user's device, confirm you meet these requirements:</span></span>

- <span data-ttu-id="e4693-104">Windows 10 x64 ビルド 1809 以降がデバイスにインストールされています。</span><span class="sxs-lookup"><span data-stu-id="e4693-104">Windows 10 x64 build 1809 or later is installed on the device.</span></span>
- <span data-ttu-id="e4693-105">マルウェア対策クライアント バージョン 4.18.2009.7 以降がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="e4693-105">Anti-malware client version 4.18.2009.7 or later is installed.</span></span>
- <span data-ttu-id="e4693-106">デバイスは次の **いずれか** です。</span><span class="sxs-lookup"><span data-stu-id="e4693-106">The device is **one** of these:</span></span>
    
    - <span data-ttu-id="e4693-107">Azure Active Directory (Azure AD) への参加</span><span class="sxs-lookup"><span data-stu-id="e4693-107">Azure Active Directory (Azure AD) joined</span></span>
    - <span data-ttu-id="e4693-108">Hybrid Azure AD への参加</span><span class="sxs-lookup"><span data-stu-id="e4693-108">Hybrid Azure AD joined</span></span>
    - <span data-ttu-id="e4693-109">AAD の登録</span><span class="sxs-lookup"><span data-stu-id="e4693-109">AAD registered</span></span>

- <span data-ttu-id="e4693-110">ポリシー アクションを適用するには、Microsoft Chromium Edge ブラウザーがエンドポイント デバイスにインストールされていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="e4693-110">To enforce policy actions, make sure Microsoft Chromium Edge browser is installed on the endpoint device.</span></span>

<span data-ttu-id="e4693-111">エンドポイント DLP を展開するための追加要件については、「[エンドポイント データ損失防止を開始する](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e4693-111">For additional requirements for deploying Endpoint DLP, see [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span></span>