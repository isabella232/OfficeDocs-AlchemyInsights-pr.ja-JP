---
title: Microsoft Edge を iOS、iPadOS、および Android に展開する
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8241"
- "9004604"
ms.openlocfilehash: 524e87ab57e29823361053093708c83831f19687
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194655"
---
# <a name="deploy-microsoft-edge-to-ios-ipados-and-android"></a><span data-ttu-id="9a70e-102">Microsoft Edge を iOS、iPadOS、および Android に展開する</span><span class="sxs-lookup"><span data-stu-id="9a70e-102">Deploy Microsoft Edge to iOS, iPadOS, and Android</span></span>

<span data-ttu-id="9a70e-103">以下に要約するガイド付きシナリオは、iOS、iPadOS、および Android デバイスのユーザーに Microsoft Edge を割り当てるのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="9a70e-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span>

> [!NOTE]
> <span data-ttu-id="9a70e-104">ユーザーがモバイル デバイスに登録できないようにした場合、このガイド シナリオは機能せず、ユーザーが Microsoft Edge を自分でインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="9a70e-104">If you blocked users from enrolling mobile devices, this guided scenario won't work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="9a70e-105">ガイド付きシナリオには、次の手順が含まれます。</span><span class="sxs-lookup"><span data-stu-id="9a70e-105">The guided scenario involves the following steps:</span></span>

1. [<span data-ttu-id="9a70e-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="9a70e-106">Prerequisites</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#prerequisites)
2. [<span data-ttu-id="9a70e-107">はじめに</span><span class="sxs-lookup"><span data-stu-id="9a70e-107">Introduction</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-1---introduction)
3. [<span data-ttu-id="9a70e-108">基本</span><span class="sxs-lookup"><span data-stu-id="9a70e-108">Basics</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-2---basics)
4. [<span data-ttu-id="9a70e-109">構成</span><span class="sxs-lookup"><span data-stu-id="9a70e-109">Configuration</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-3---configuration)
5. [<span data-ttu-id="9a70e-110">割り当て</span><span class="sxs-lookup"><span data-stu-id="9a70e-110">Assignments</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-4---assignments)
6. [<span data-ttu-id="9a70e-111">レビューと作成</span><span class="sxs-lookup"><span data-stu-id="9a70e-111">Review and creation</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-5---review--create)

<span data-ttu-id="9a70e-112">ガイド付きシナリオの手順を完了すると、Microsoft Intune ポリシーにより、Microsoft Edge for Business の次の機能が有効になります。</span><span class="sxs-lookup"><span data-stu-id="9a70e-112">After you complete the steps in the guided scenario, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="9a70e-113">デュアル ID</span><span class="sxs-lookup"><span data-stu-id="9a70e-113">Dual identity</span></span>
- <span data-ttu-id="9a70e-114">Microsoft Intune アプリ保護ポリシーとの統合</span><span class="sxs-lookup"><span data-stu-id="9a70e-114">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="9a70e-115">Azure Active Directory アプリケーション プロキシとの統合</span><span class="sxs-lookup"><span data-stu-id="9a70e-115">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="9a70e-116">管理されたお気に入りとホーム ページのショートカット</span><span class="sxs-lookup"><span data-stu-id="9a70e-116">Managed favorites and home page shortcuts</span></span>
