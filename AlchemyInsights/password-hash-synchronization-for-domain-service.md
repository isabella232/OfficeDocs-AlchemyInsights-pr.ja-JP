---
title: ドメイン サービスのパスワード ハッシュ同期
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
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177820"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="408e8-102">ドメイン サービスのパスワード ハッシュ同期</span><span class="sxs-lookup"><span data-stu-id="408e8-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="408e8-103">**Azure AD DS インスタンスがパスワード ハッシュ同期を有効にするように要求している場合**</span><span class="sxs-lookup"><span data-stu-id="408e8-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="408e8-104">オンプレミスの Azure Active Directory Domain Services (AD DS) 環境からユーザーが同期するハイブリッド環境を実行しているシナリオが発生します。</span><span class="sxs-lookup"><span data-stu-id="408e8-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="408e8-105">このシナリオは、オンプレミス AD DS から Azure AD テナントへのパスワード ハッシュ同期があるにもかかわらず発生します。</span><span class="sxs-lookup"><span data-stu-id="408e8-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="408e8-106">**原因**</span><span class="sxs-lookup"><span data-stu-id="408e8-106">**Cause**</span></span>

<span data-ttu-id="408e8-107">これは、Azure AD Connect が既定で、Azure AD DS に必要な従来の New Technology LAN Manager (NTLM) と Kerberos パスワード ハッシュを同期しないために発生します。</span><span class="sxs-lookup"><span data-stu-id="408e8-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="408e8-108">**回避策**</span><span class="sxs-lookup"><span data-stu-id="408e8-108">**Workaround**</span></span> 

<span data-ttu-id="408e8-109">NTLM および Kerberos 認証に必要なパスワード ハッシュを同期するように Azure AD Connect を構成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="408e8-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="408e8-110">Azure AD Connect が構成された後、オンプレミスのアカウント作成またはパスワード変更イベントも、従来のパスワード ハッシュを Azure AD に同期します。</span><span class="sxs-lookup"><span data-stu-id="408e8-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="408e8-111">これに関する詳細情報と、Azure AD DS ハイブリッド環境でパスワード同期を有効にする方法のガイダンスについては、[こちら](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="408e8-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>