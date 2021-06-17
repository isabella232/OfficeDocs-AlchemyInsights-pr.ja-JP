---
title: Active Directory が同期しない
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
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930980"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="1bad1-102">Active Directory が同期しない</span><span class="sxs-lookup"><span data-stu-id="1bad1-102">Active Directory not syncing</span></span>

<span data-ttu-id="1bad1-103">「同期が最近行われていません」などの同期エラーが表示される場合、または Office 管理ポータルでディレクトリ同期の状態が「最後の同期: 3 日以上前」と表示される場合は、AADConnect の設定が正しくないか、同期を実行するための権限が不十分である可能性があります。</span><span class="sxs-lookup"><span data-stu-id="1bad1-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="1bad1-104">[簡単設定] を使用して AADConnect を再インストールすると、すぐに問題が解決する場合があります。</span><span class="sxs-lookup"><span data-stu-id="1bad1-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="1bad1-105">[AADConnect の最新バージョンをダウンロードします](https://go.microsoft.com/fwlink/?LinkId=615771)。</span><span class="sxs-lookup"><span data-stu-id="1bad1-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="1bad1-106">[高速インストール手順に従います](/azure/active-directory/hybrid/how-to-connect-install-express)。</span><span class="sxs-lookup"><span data-stu-id="1bad1-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="1bad1-107">Azure AD Connect は、Windows Server 2012 以降にインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="1bad1-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="1bad1-108">このサーバーはドメイン参加型である必要があり、ドメイン コントローラーまたはメンバー サーバーの場合があります。</span><span class="sxs-lookup"><span data-stu-id="1bad1-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="1bad1-109">Azure AD Connect の要件と前提条件の完全なリストについては、[Azure AD Connect の前提条件](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="1bad1-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="1bad1-110">AADConnect サービス アカウントの詳細については、「[Azure AD Connect: アカウントとアクセス許可](/azure/active-directory/hybrid/reference-connect-accounts-permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1bad1-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
