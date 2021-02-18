---
title: グループ ポリシー
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/15/2021
ms.locfileid: "50257015"
---
# <a name="group-policy"></a><span data-ttu-id="22fd2-102">グループ ポリシー</span><span class="sxs-lookup"><span data-stu-id="22fd2-102">Group policy</span></span>

<span data-ttu-id="22fd2-103">Azure Active Directory Domain Services (Azure AD DS) のユーザー オブジェクトとコンピューター オブジェクトの設定は、多くの場合、グループ ポリシー オブジェクト (GPO) を使用して管理されます。</span><span class="sxs-lookup"><span data-stu-id="22fd2-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="22fd2-104">Azure AD DS には、AADDC Users コンテナーおよび AADDC Computers コンテナー用の組み込み GPO が含まれています。</span><span class="sxs-lookup"><span data-stu-id="22fd2-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="22fd2-105">これらの組み込みの GPO をカスタマイズして、環境のニーズに合わせてグループ ポリシーを構成できます。</span><span class="sxs-lookup"><span data-stu-id="22fd2-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="22fd2-106">Azure AD DC 管理者 グループのメンバーは、Azure AD DS ドメイン内でグループ ポリシー管理特権を持っています。また、カスタムの GPO と組織単位 (OU) を作成することもできます。</span><span class="sxs-lookup"><span data-stu-id="22fd2-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="22fd2-107">グループ ポリシーとそのしくみの詳細については、「[グループ ポリシーの概要](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="22fd2-107">For more information on what group policy is and how it works, see [Group Policy overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="22fd2-108">ハイブリッド環境では、オンプレミスの AD DS 環境内で構成されているグループ ポリシーは、Azure AD DS に同期されません。</span><span class="sxs-lookup"><span data-stu-id="22fd2-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="22fd2-109">Azure AD DS のユーザーまたはコンピューターの構成設定を定義するには、既定のいずれかの GPO を編集するか、カスタム GPO を作成します。</span><span class="sxs-lookup"><span data-stu-id="22fd2-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="22fd2-110">こちらの記事「[グループ ポリシーの管理](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy)」では、グループ ポリシー管理ツールのインストール方法、組み込みの GPO の編集方法、カスタム GPO の作成方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="22fd2-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>



