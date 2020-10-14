---
title: BlockLegacyAuth
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
- "3154"
- "9001194"
ms.openlocfilehash: baf3ee808cce1e4da362dd0841c0138d7d9268d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685603"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="aff84-102">レガシ認証のブロック</span><span class="sxs-lookup"><span data-stu-id="aff84-102">Blocking legacy authentication</span></span>

<span data-ttu-id="aff84-103">レガシ認証とは、以下によって行われる認証要求を指す用語です。</span><span class="sxs-lookup"><span data-stu-id="aff84-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="aff84-104">モダンな認証を使用しない、以前のバージョンの Office クライアント (Office 2010 クライアントなど)。</span><span class="sxs-lookup"><span data-stu-id="aff84-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="aff84-105">IMAP/S MTP/POP3 などのレガシ メール プロトコルを使用するクライアント。</span><span class="sxs-lookup"><span data-stu-id="aff84-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="aff84-106">レガシ認証のブロックおよびモダンな認証の有効化の詳細については、「[レガシ認証のブロック](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aff84-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="aff84-107">Azure Active Directory (Azure AD) のセキュリティの既定値は、セキュリティの確保を容易にし、組織の保護に貢献します。</span><span class="sxs-lookup"><span data-stu-id="aff84-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="aff84-108">セキュリティの既定値には、一般的な攻撃に関する事前構成済みのセキュリティ設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="aff84-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="aff84-109">セキュリティの既定値の詳細については、「[セキュリティの既定値とは](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aff84-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="aff84-110">**注**: 2019 年 10 月 22 日以降に作成されたテナントの場合、既定でセキュリティ保護されている新しい動作になっており、テナントで既にセキュリティの既定値が有効になっている可能性があります。</span><span class="sxs-lookup"><span data-stu-id="aff84-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="aff84-111">すべてのユーザーを保護するために、セキュリティの既定値は、新しく作成されるすべてのテナントに展開されています。</span><span class="sxs-lookup"><span data-stu-id="aff84-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
