---
title: セキュリティ グループの問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177821"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="51f12-102">セキュリティ グループの問題</span><span class="sxs-lookup"><span data-stu-id="51f12-102">Issue with security groups</span></span>

<span data-ttu-id="51f12-103">**ネットワーク エラー AADDS104 が発生した場合**</span><span class="sxs-lookup"><span data-stu-id="51f12-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="51f12-104">無効なネットワーク セキュリティ グループ ルールは、Azure Active Directory Domain Services (AD DS) のネットワーク エラーの最も一般的な原因です。</span><span class="sxs-lookup"><span data-stu-id="51f12-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="51f12-105">仮想ネットワークのネットワーク セキュリティ グループは、特定のポートとプロトコルへのアクセスを許可する必要があります。</span><span class="sxs-lookup"><span data-stu-id="51f12-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="51f12-106">これらのポートがブロックされている場合、Azure プラットフォームは管理対象ドメインを監視または更新できません。</span><span class="sxs-lookup"><span data-stu-id="51f12-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="51f12-107">Azure AD と Azure AD DS 間の同期も影響を受けます。</span><span class="sxs-lookup"><span data-stu-id="51f12-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="51f12-108">サービスの中断を避けるために、既定のポートを開いたままにしてください。</span><span class="sxs-lookup"><span data-stu-id="51f12-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="51f12-109">ネットワーク セキュリティ グループの構成の問題に関する一般的なアラートを理解して解決するには、「[セキュリティ グループの追加と確認](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="51f12-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
