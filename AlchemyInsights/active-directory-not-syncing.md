---
title: Active Directory が同期しない
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/25/2020
ms.locfileid: "42268953"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="fdab2-102">Active Directory が同期しない</span><span class="sxs-lookup"><span data-stu-id="fdab2-102">Active Directory not syncing</span></span>

<span data-ttu-id="fdab2-103">"最近の同期がありません" のような同期エラーを受信している場合、または Office 管理ポータルのディレクトリ同期の状態が "前回の同期は3日前" であることが示されている場合は、AADConnect の設定が正しくないか、または不足している可能性があります。同期を実行するためのアクセス許可。</span><span class="sxs-lookup"><span data-stu-id="fdab2-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="fdab2-104">エクスプレス設定を使用して AADConnect を再インストールすると、問題が迅速に解決する場合があります。</span><span class="sxs-lookup"><span data-stu-id="fdab2-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="fdab2-105">[AADConnect の最新バージョンをダウンロード](https://go.microsoft.com/fwlink/?LinkId=615771)します。</span><span class="sxs-lookup"><span data-stu-id="fdab2-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="fdab2-106">[高速インストールの手順に従い](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)ます。</span><span class="sxs-lookup"><span data-stu-id="fdab2-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="fdab2-107">AADConnect サービスアカウントの詳細については、「 [AZURE AD Connect: accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fdab2-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
