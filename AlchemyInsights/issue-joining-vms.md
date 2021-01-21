---
title: VM への参加の問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885822"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="887c7-102">VM への参加の問題</span><span class="sxs-lookup"><span data-stu-id="887c7-102">Issue joining VMs</span></span>

<span data-ttu-id="887c7-103">VM への参加中に発生する問題を解決するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="887c7-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="887c7-104">**SAMAccountName** 形式 (「CONTOSO\joeuser」) の代わりに **UPN** 形式 (たとえば、「joeuser@contoso.com」) を使用してサインインしてみてください。</span><span class="sxs-lookup"><span data-stu-id="887c7-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="887c7-105">*作業の開始* ガイドに記載されている手順に従って、パスワードの同期が有効になっていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="887c7-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="887c7-106">影響を受けるユーザー アカウントが Azure AD テナントの外部アカウントでないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="887c7-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="887c7-107">Azure AD Domain Services には管理対象ドメインの資格情報がないため、外部ユーザーは管理対象ドメインにサインインできません。</span><span class="sxs-lookup"><span data-stu-id="887c7-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="887c7-108">影響を受けるユーザー アカウントがクラウド専用のユーザー アカウントの場合は、Azure AD Domain Services を有効にした後でユーザーがパスワードを変更したことを確認します。</span><span class="sxs-lookup"><span data-stu-id="887c7-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="887c7-109">この手順により、Azure AD Domain Services に必要な資格情報ハッシュが生成されます。</span><span class="sxs-lookup"><span data-stu-id="887c7-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="887c7-110">影響を受けるユーザー アカウントがオンプレミス ディレクトリから同期される場合は、Azure AD Connect の推奨リリースが完全同期を実行するように構成されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="887c7-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="887c7-111">手順 4 を確認しても問題が解決しない場合は、同期マシンから次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="887c7-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="887c7-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="887c7-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>