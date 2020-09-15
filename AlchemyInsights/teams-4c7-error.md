---
title: Teams 4c7 エラー
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
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700208"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="7ce3c-102">Microsoft Teams の 4c7 エラー</span><span class="sxs-lookup"><span data-stu-id="7ce3c-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="7ce3c-103">このエラーは、Microsoft Teams でフォーム認証が必要な場合に発生します。</span><span class="sxs-lookup"><span data-stu-id="7ce3c-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="7ce3c-104">Active Directory フェデレーション サービス (AD FS) を展開した場合、既定では、フォーム認証がイントラネットに対して有効になっていません。</span><span class="sxs-lookup"><span data-stu-id="7ce3c-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="7ce3c-105">Windows 統合認証に失敗した場合は、フォーム認証を使用してサインインするように求められます。</span><span class="sxs-lookup"><span data-stu-id="7ce3c-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="7ce3c-106">この問題を解決するには、Active Directory のローカル コピーがあるコンピューターで AD FS Microsoft 管理コンソール (MMC) スナップインを使用して、フォーム認証を有効にします。</span><span class="sxs-lookup"><span data-stu-id="7ce3c-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="7ce3c-107">これを行うには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="7ce3c-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="7ce3c-108">ナビゲーション ウィンドウで、「**認証ポリシー**」を参照します。</span><span class="sxs-lookup"><span data-stu-id="7ce3c-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="7ce3c-109">詳細ウィンドウの [**アクション**] で、[**グローバル プライマリ認証の編集**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7ce3c-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="7ce3c-110">[**イントラネット**] タブで、[**フォーム認証**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="7ce3c-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="7ce3c-111">[**OK**] (または [**適用**]) を選択します。</span><span class="sxs-lookup"><span data-stu-id="7ce3c-111">Select **OK** (or **Apply**).</span></span>