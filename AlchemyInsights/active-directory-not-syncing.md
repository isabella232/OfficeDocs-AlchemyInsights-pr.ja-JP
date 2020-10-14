---
title: Active Directory が同期しない
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
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697634"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="91d3d-102">Active Directory が同期しない</span><span class="sxs-lookup"><span data-stu-id="91d3d-102">Active Directory not syncing</span></span>

<span data-ttu-id="91d3d-103">「同期が最近行われていません」などの同期エラーが表示される場合、または Office 管理ポータルでディレクトリ同期の状態が「最後の同期: 3 日以上前」と表示される場合は、AADConnect の設定が正しくないか、同期を実行するための権限が不十分である可能性があります。</span><span class="sxs-lookup"><span data-stu-id="91d3d-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="91d3d-104">[簡単設定] を使用して AADConnect を再インストールすると、すぐに問題が解決する場合があります。</span><span class="sxs-lookup"><span data-stu-id="91d3d-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="91d3d-105">[AADConnect の最新バージョンをダウンロードします](https://go.microsoft.com/fwlink/?LinkId=615771)。</span><span class="sxs-lookup"><span data-stu-id="91d3d-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="91d3d-106">[高速インストール手順に従います](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)。</span><span class="sxs-lookup"><span data-stu-id="91d3d-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="91d3d-107">AADConnect サービス アカウントの詳細については、「[Azure AD Connect: アカウントとアクセス許可](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="91d3d-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
