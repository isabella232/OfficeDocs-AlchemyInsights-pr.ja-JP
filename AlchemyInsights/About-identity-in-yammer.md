---
title: Yammer の ID について
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664175"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="dcdca-102">Yammer の ID について</span><span class="sxs-lookup"><span data-stu-id="dcdca-102">About identity in Yammer</span></span>

<span data-ttu-id="dcdca-103">ID 関連の問題を回避するために、すべてのネットワークで次の手順を実行することをお勧めします:</span><span class="sxs-lookup"><span data-stu-id="dcdca-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="dcdca-104">Azure AD のユーザーに Microsoft 365 アカウントをプロビジョニングした後に Office 365 ID を適用して、すべてのユーザーが主要な Microsoft 365 アカウントを使用してサインインするようにします。</span><span class="sxs-lookup"><span data-stu-id="dcdca-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="dcdca-105">詳しくは、[「Yammer ユーザーに Office 365 ID を適用する」](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dcdca-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="dcdca-106">複数の Yammer ネットワークを統合します。</span><span class="sxs-lookup"><span data-stu-id="dcdca-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="dcdca-107">従来の Yammer 構成では、1 つのテナントに複数の Yammer ネットワークを接続できます。</span><span class="sxs-lookup"><span data-stu-id="dcdca-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="dcdca-108">詳しくは、[「ネットワークの移行 - 複数の Yammer ネットワークを統合する」](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dcdca-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="dcdca-109">必要に応じて、ユーザーにライセンスがない場合に Yammer からユーザーをブロックするために、Yammer にライセンスを適用します。</span><span class="sxs-lookup"><span data-stu-id="dcdca-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="dcdca-110">詳しくは、[「Office 365 で Yammer ユーザー ライセンスを管理する」](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dcdca-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="dcdca-111">最後に、以前の Yammer ネットワークのユーザー リストを監査し、従来のユーザーを一時停止します。</span><span class="sxs-lookup"><span data-stu-id="dcdca-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="dcdca-112">削除は元に戻せないため、ユーザーを削除するのではなく、一時停止 （非アクティブ化） することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="dcdca-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="dcdca-113">詳しくは、[「Office 365 に接続されているネットワークで Yammer ユーザーを監査する」](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) と [「ユーザーを削除する」](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dcdca-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="dcdca-114">これらの手順を使用して Yammer を構成すると、Microsoft 365 のネイティブ モードで Yammer ネットワークを構成する準備ができます。</span><span class="sxs-lookup"><span data-stu-id="dcdca-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="dcdca-115">詳しくは、[「Microsoft 365 のネイティブ モードで Yammer ネットワークを構成する」](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dcdca-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>