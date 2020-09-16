---
title: 従来の電子情報開示ツールの廃止
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
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727788"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="3c7d0-102">従来の電子情報開示ツールの廃止</span><span class="sxs-lookup"><span data-stu-id="3c7d0-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="3c7d0-103">Microsoft 365 コンプライアンス センターの電子情報開示機能が刷新され、機能が向上したことにより、次に挙げる従来の電子情報開示ツールおよびコマンドレットは今後数か月間の間に廃止されます。</span><span class="sxs-lookup"><span data-stu-id="3c7d0-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="3c7d0-104">Exchange 管理センターの[インプレース電子情報開示](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery)および[インプレース ホールド](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)。</span><span class="sxs-lookup"><span data-stu-id="3c7d0-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="3c7d0-105">インプレース電子情報開示およびインプレース ホールドをサポートしている、Exchange Online の PowerShell コマンドレット。</span><span class="sxs-lookup"><span data-stu-id="3c7d0-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="3c7d0-106">(これらのコマンドレットは、まとめて \*-MailboxSearch cmdlets と識別されます。) 次のコマンドレットが含まれます。</span><span class="sxs-lookup"><span data-stu-id="3c7d0-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="3c7d0-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="3c7d0-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="3c7d0-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="3c7d0-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="3c7d0-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="3c7d0-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="3c7d0-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="3c7d0-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="3c7d0-111">Exchange Online PowerShell の [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) コマンドレット。</span><span class="sxs-lookup"><span data-stu-id="3c7d0-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="3c7d0-112">Exchange Web Services API での次の操作。</span><span class="sxs-lookup"><span data-stu-id="3c7d0-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="3c7d0-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="3c7d0-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="3c7d0-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="3c7d0-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="3c7d0-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="3c7d0-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="3c7d0-116">Advanced eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="3c7d0-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="3c7d0-117">**廃止のタイムライン**:</span><span class="sxs-lookup"><span data-stu-id="3c7d0-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="3c7d0-118">**2020 年 7 月 1 日**: 新しい検索と保留リストを作成できなくなりますが、ユーザーの自己責任において、既存の検索の実行、編集、および削除は行えます。</span><span class="sxs-lookup"><span data-stu-id="3c7d0-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="3c7d0-119">Microsoft サポートによる Exchange 管理センターのインプレース電子情報開示およびインプレース ホールドのサポートが終了します。</span><span class="sxs-lookup"><span data-stu-id="3c7d0-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="3c7d0-120">**2020 年 10 月 1 日**: EAC のインプレース電子情報開示と保持機能は読み取り専用モードになるため、既存の検索と保持のみを削除できます。</span><span class="sxs-lookup"><span data-stu-id="3c7d0-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="3c7d0-121">**詳細については、以下を参照してください。**</span><span class="sxs-lookup"><span data-stu-id="3c7d0-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="3c7d0-122">従来の電子情報開示検索と保持を Microsoft 365 コンプライアンス センターに移行する</span><span class="sxs-lookup"><span data-stu-id="3c7d0-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="3c7d0-123">従来の電子情報開示ツールの廃止</span><span class="sxs-lookup"><span data-stu-id="3c7d0-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="3c7d0-124">インプレース電子情報開示とインプレース ホールドに関するよくある質問</span><span class="sxs-lookup"><span data-stu-id="3c7d0-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



