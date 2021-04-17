---
title: グループを作成する
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
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816361"
---
# <a name="create-a-group"></a><span data-ttu-id="312f2-102">グループを作成する</span><span class="sxs-lookup"><span data-stu-id="312f2-102">Create a group</span></span>

<span data-ttu-id="312f2-103">このトピックでは、グループの作成について説明します。</span><span class="sxs-lookup"><span data-stu-id="312f2-103">This topic describes group creation.</span></span>

<span data-ttu-id="312f2-104">**グループを作成する権限**</span><span class="sxs-lookup"><span data-stu-id="312f2-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="312f2-105">新しいグループを作成する権限があることを確認します。</span><span class="sxs-lookup"><span data-stu-id="312f2-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="312f2-106">グローバル管理者は、Azure ポータルまたはアクセス パネルでグループの作成を無効にできます。</span><span class="sxs-lookup"><span data-stu-id="312f2-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="312f2-107">新しいグループを作成したり、適切な権限を付与したりするには、管理者が必要になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="312f2-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="312f2-108">**グループ作成の権限の管理**</span><span class="sxs-lookup"><span data-stu-id="312f2-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="312f2-109">グローバル管理者は、**[すべてのグループ]** >  **[全般 (設定)]** で「ユーザーは Azure ポータルでセキュリティ グループを作成できます」または「ユーザーは Azure ポータルで Office 365 グループを作成できます」オプションを選択することにより、グループ作成のアクセス許可 (セキュリティ上の理由)、Azure ポータル、またはアクセスパネルで作成された Office 365 グループを管理できます。</span><span class="sxs-lookup"><span data-stu-id="312f2-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="312f2-110">Azure Active Directory P1 Premium ライセンスをお持ちの場合は、グループの作成を制限してユーザーのグループを選択することもできます。</span><span class="sxs-lookup"><span data-stu-id="312f2-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="312f2-111">**新しい Office 365 グループメンバーのウェルカム通知を無効にする**</span><span class="sxs-lookup"><span data-stu-id="312f2-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="312f2-112">Office 365 グループに追加されたユーザーに送信されるウェルカム通知を無効にするには、Powershell で **UnifiedGroupWelcomeMessageEnabled** を False に設定します。</span><span class="sxs-lookup"><span data-stu-id="312f2-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="312f2-113">この設定については、[こちら](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="312f2-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

