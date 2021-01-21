---
title: 'ドメイン コントローラ '
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901720"
---
# <a name="domain-controller"></a><span data-ttu-id="c8ec5-102">ドメイン コントローラ</span><span class="sxs-lookup"><span data-stu-id="c8ec5-102">Domain controller</span></span>

<span data-ttu-id="c8ec5-103">**AAD-DS を有効にできないか、展開が失敗しています**</span><span class="sxs-lookup"><span data-stu-id="c8ec5-103">**Unable to enable AAD-DS or deployment is failing**</span></span>

<span data-ttu-id="c8ec5-104">Azure AD Domain Services (AAD-DS) が有効になっていない、または展開できない問題を解決するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="c8ec5-104">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="c8ec5-105">既存の仮想ネットワークを使用している場合は、ポータル https://aka.ms/aadds-networking の AAD-DS で同期するために必要なポートをブロックする規則がないか NSG を確認します。</span><span class="sxs-lookup"><span data-stu-id="c8ec5-105">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="c8ec5-106">エラー メッセージが、https://aka.ms/aadds-troubleshoot-enable で利用可能なこのトラブルシューティング ガイドに記載されているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="c8ec5-106">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="c8ec5-107">新しい仮想ネットワークに Azure AD Domain Services を展開してみます。</span><span class="sxs-lookup"><span data-stu-id="c8ec5-107">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="c8ec5-108">[Azure AD ドメイン サービスを作成するためのチュートリアル](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)で利用できる AAD-DS の展開方法については、「作業の開始ガイド」に従ってください。</span><span class="sxs-lookup"><span data-stu-id="c8ec5-108">Follow the Getting Started guide on how to deploy AAD-DS, which is available at [Tutorial to Create Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="c8ec5-109">Azure AD Domain Services の展開に問題がある場合は、「[Azure AD Domain Services のトラブルシューティング](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)」を参照して、作業を再開するための一般的なエラーを解決してください。</span><span class="sxs-lookup"><span data-stu-id="c8ec5-109">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="c8ec5-110">**AAD-DS を無効にできない**</span><span class="sxs-lookup"><span data-stu-id="c8ec5-110">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="c8ec5-111">AD-DS を一時停止できません。</span><span class="sxs-lookup"><span data-stu-id="c8ec5-111">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="c8ec5-112">管理対象ドメインの使用を停止する場合は、ドメインを削除する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8ec5-112">If you wish to stop using your managed domain, it must be deleted.</span></span>

<span data-ttu-id="c8ec5-113">問題が発生した場合、一般的なエラー メッセージを解決するため、および関連するトラブルシューティングの手順については、「[Azure ActiveDirectoryドメインサービスのトラブルシューティング](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c8ec5-113">If you run into issues, to resolve common error messages and for associated troubleshooting steps to help you get things running again, see [Troubleshoot Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span></span>
