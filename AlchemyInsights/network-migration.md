---
title: ネットワークの移行
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "716"
- "6000002"
ms.assetid: b5ab885c-3803-4cc8-adab-94848e226ffb
ms.openlocfilehash: 6f026f932bb35d12d32ce7eddf49e49a44db7f31
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799569"
---
# <a name="network-migration"></a><span data-ttu-id="ab4aa-102">ネットワークの移行</span><span class="sxs-lookup"><span data-stu-id="ab4aa-102">Network Migration</span></span>

<span data-ttu-id="ab4aa-p101">ご使用の O365 テナントは 1 つのテナント内で複数の Yammer ネットワークに関連付けられている可能性があります (多数のネットワーク構成)。2018 年 10 月 16 日以降、Yammer は 1 つのテナントへの複数の Yammer ネットワークの関連付けをサポートしなくなりました。ネットワークの移行を行うことで、適切な 1 対 1 構成にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ab4aa-p101">Your O365 tenant is possibly associated with multiple Yammer networks in a 1 tenant : Many networks configuration. Starting October 16, 2018, Yammer will no longer support multiple Yammer networks associated with one tenant. You can perform a Network Migration to get to a preferred 1:1 configuration.</span></span>
  
- <span data-ttu-id="ab4aa-p102">ご使用のテナントに関連付けられているネットワークのリストを表示するには、グローバル管理者として Yammer にログインし、**[ネットワーク管理者]**、**[ネットワーク移行]** の順に参照します。**[次へ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="ab4aa-p102">To view a list of the networks associated with your tenant, log in to Yammer as an Global Administrator and browse to **Network Admin**, then **Network Migration**. Choose **Next**.</span></span>

- <span data-ttu-id="ab4aa-108">手順 2/3 で複数のネットワークが一覧表示される場合は、ご使用の O365 テナントに複数のネットワークが関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="ab4aa-108">If you see multiple networks listed on Step 2 of 3, then you have multiple Yammer networks associated with your O365 tenant.</span></span>

- <span data-ttu-id="ab4aa-109">構成を 1 対 1 に修正するには、引き続きネットワーク移行ツールを使用します。</span><span class="sxs-lookup"><span data-stu-id="ab4aa-109">To correct your configuration to a 1:1 configuration, continue using the Network Migration tool.</span></span>

- <span data-ttu-id="ab4aa-110">ネットワーク移行の詳細については、「[ネットワークの移行: 複数の Yammer ネットワークの統合](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ab4aa-110">For more information on Network Migration please see [Network migration: Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>

<span data-ttu-id="ab4aa-111">次の点にご注意ください。</span><span class="sxs-lookup"><span data-stu-id="ab4aa-111">Please Note:</span></span>
  
- <span data-ttu-id="ab4aa-p103">**ネットワークの移行では、アクティブなユーザーおよび保留中のユーザーのみが移行されます。** アクティブなユーザーと共に、名前やプロファイル画像などのユーザー情報も移行されます。グループなどのネットワーク コンテンツは移行されません。</span><span class="sxs-lookup"><span data-stu-id="ab4aa-p103">**A network migration migrates only the active and pending users.** Along with the active users, the users' information, such as name and profile picture, is also migrated. Any network content, including groups, is not migrated.</span></span>

- <span data-ttu-id="ab4aa-p104">**ネットワークの移行を取り消すことはできません。** 移行後は、ご使用の従属ネットワークとそのコンテンツにアクセスできなくなります。そのため、移行を検討する前に、慎重に計画を立てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="ab4aa-p104">**Network migration can't be reversed.** You will not be able to access your subsidiary network and its content after migration. So before you consider a migration, you want to plan carefully.</span></span>
