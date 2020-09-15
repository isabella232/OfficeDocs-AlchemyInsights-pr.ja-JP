---
title: 孤立したユーザーをオンプレミスサーバーから削除する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 537ae7edebfa5a4ab71c2141d549d732ed4f883f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680140"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a><span data-ttu-id="c9e84-102">孤立したユーザーをオンプレミスサーバーから削除する</span><span class="sxs-lookup"><span data-stu-id="c9e84-102">Delete orphaned user from on-premises server</span></span>

<span data-ttu-id="c9e84-103">次の手順に従い、孤立したユーザーを削除します。</span><span class="sxs-lookup"><span data-stu-id="c9e84-103">To remove an orphaned user, follow these steps:</span></span>

1. <span data-ttu-id="c9e84-104">「[Azure Active Directory でのハイブリッド ID とは?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories)」の手順に従い、ディレクトリ同期を強制します。</span><span class="sxs-lookup"><span data-stu-id="c9e84-104">Force directory synchronization by following the instructions in [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).</span></span>

2. <span data-ttu-id="c9e84-105">ディレクトリ同期を確認するには、「[Azure Active Directory でのハイブリッド ID とは?](https://technet.microsoft.com/library/jj151797.aspx)」を参照します。</span><span class="sxs-lookup"><span data-stu-id="c9e84-105">To verify directory synchronization, see [What is hybrid identity with Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).</span></span>

3. <span data-ttu-id="c9e84-106">同期は正しく機能するが、Active Directory オブジェクトの削除が Azure AD に反映されない場合は、次の Windows PowerShell コマンドレット用 Azure Active Directory モジュールのいずれかを使用して、孤立したオブジェクトを手動で削除します。</span><span class="sxs-lookup"><span data-stu-id="c9e84-106">If sync functions correctly but the Active Directory object deletion does not propagate to Azure AD, manually remove the orphaned object by using one of the following Azure Active Directory Module for Windows PowerShell cmdlets:</span></span>

    <span data-ttu-id="c9e84-107">Remove-MsolContact</span><span class="sxs-lookup"><span data-stu-id="c9e84-107">Remove-MsolContact</span></span>  
    <span data-ttu-id="c9e84-108">Remove-MsolGroup</span><span class="sxs-lookup"><span data-stu-id="c9e84-108">Remove-MsolGroup</span></span>  
    <span data-ttu-id="c9e84-109">Remove-MsolUser</span><span class="sxs-lookup"><span data-stu-id="c9e84-109">Remove-MsolUser</span></span>

    <span data-ttu-id="c9e84-110">例えば、元はディレクトリ同期を使用して作成された孤立したユーザーID john.smith@contoso.com を削除するには、次のコマンドレットを実行します。</span><span class="sxs-lookup"><span data-stu-id="c9e84-110">For example, to remove orphaned user ID john.smith@contoso.com, originally created by using directory synchronization, run the cmdlet:</span></span>

    <span data-ttu-id="c9e84-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="c9e84-111">Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com</span></span>