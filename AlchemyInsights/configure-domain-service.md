---
title: Domain Services の構成
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
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885824"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="27e1e-102">AAD-DS を有効にできないか、展開に失敗する</span><span class="sxs-lookup"><span data-stu-id="27e1e-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="27e1e-103">Azure AD Domain Services (AAD-DS) が有効になっていない、または展開できない問題を解決するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="27e1e-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="27e1e-104">既存の仮想ネットワークを使用している場合は、ポータル https://aka.ms/aadds-networking の AAD-DS で同期するために必要なポートをブロックする規則がないか NSG を確認します。</span><span class="sxs-lookup"><span data-stu-id="27e1e-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="27e1e-105">エラー メッセージが、https://aka.ms/aadds-troubleshoot-enable で利用可能なこのトラブルシューティング ガイドに記載されているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="27e1e-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="27e1e-106">新しい仮想ネットワークに Azure AD Domain Services を展開してみます。</span><span class="sxs-lookup"><span data-stu-id="27e1e-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="27e1e-107">AAD-DS の展開方法については、「[AAD Domain Services の作成と構成](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)」で作業の開始ガイドに従います。</span><span class="sxs-lookup"><span data-stu-id="27e1e-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="27e1e-108">Azure AD Domain Services の展開に問題がある場合は、「[Azure AD Domain Services のトラブルシューティング](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)」を参照して、作業を再開するための一般的なエラーを解決してください。</span><span class="sxs-lookup"><span data-stu-id="27e1e-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="27e1e-109">**AAD-DS を無効にできない**</span><span class="sxs-lookup"><span data-stu-id="27e1e-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="27e1e-110">AD-DS を一時停止できません。</span><span class="sxs-lookup"><span data-stu-id="27e1e-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="27e1e-111">管理対象ドメインの使用を停止する場合は、ドメインを削除する必要があります。</span><span class="sxs-lookup"><span data-stu-id="27e1e-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="27e1e-112">管理対象ドメインを削除するには、「[AAD Domain Services の削除](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="27e1e-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>



