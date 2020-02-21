---
title: 従来の電子情報開示ツールの廃止
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: c4632b52dde579b7d5b2e6e15f1583300a0bd136
ms.sourcegitcommit: a7c17217c170ead24571421baaf5a14f1525b1a6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158090"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="755e9-102">従来の電子情報開示ツールの廃止</span><span class="sxs-lookup"><span data-stu-id="755e9-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="755e9-103">Microsoft 365 コンプライアンスセンターの新機能と改善された電子情報開示機能の結果として、次の従来の電子情報開示ツールおよびコマンドレットを使用すると、今後数か月で廃止されることになります。</span><span class="sxs-lookup"><span data-stu-id="755e9-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="755e9-104">Exchange 管理センターでは、[インプレース電子情報開示](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery)と[インプレース保持](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)が行われます。</span><span class="sxs-lookup"><span data-stu-id="755e9-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="755e9-105">インプレース電子情報開示とインプレース保持をサポートする Exchange Online の PowerShell コマンドレット。</span><span class="sxs-lookup"><span data-stu-id="755e9-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="755e9-106">(これらのコマンドレットは、Get-mailboxsearch コマンドレットと総称して識別されます。)これには、次のコマンドレットが含まれます。</span><span class="sxs-lookup"><span data-stu-id="755e9-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="755e9-107">Get-mailboxsearch</span><span class="sxs-lookup"><span data-stu-id="755e9-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="755e9-108">Get-mailboxsearch</span><span class="sxs-lookup"><span data-stu-id="755e9-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="755e9-109">Get-mailboxsearch</span><span class="sxs-lookup"><span data-stu-id="755e9-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="755e9-110">Get-mailboxsearch</span><span class="sxs-lookup"><span data-stu-id="755e9-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="755e9-111">Exchange Online PowerShell の[検索-メールボックス](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps)コマンドレット。</span><span class="sxs-lookup"><span data-stu-id="755e9-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="755e9-112">Exchange Web サービス API の次の操作。</span><span class="sxs-lookup"><span data-stu-id="755e9-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="755e9-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="755e9-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="755e9-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="755e9-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="755e9-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="755e9-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="755e9-116">Office 365 Advanced eDiscovery version 1.0</span><span class="sxs-lookup"><span data-stu-id="755e9-116">Office 365 Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="755e9-117">**定年後のタイムライン**:</span><span class="sxs-lookup"><span data-stu-id="755e9-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="755e9-118">2020年4月1日: 新しい検索と保持を作成することはできませんが、既存の検索を自分のリスクで実行、編集、削除することはできます。</span><span class="sxs-lookup"><span data-stu-id="755e9-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="755e9-119">Microsoft サポートは、EAC でインプレース電子情報開示 & 保持をサポートしなくなります。</span><span class="sxs-lookup"><span data-stu-id="755e9-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="755e9-120">2020年7月1日: インプレース電子情報開示 & は、EAC の機能を読み取り専用モードで保持します。</span><span class="sxs-lookup"><span data-stu-id="755e9-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="755e9-121">これは、既存の検索と保持を削除できることを意味します。</span><span class="sxs-lookup"><span data-stu-id="755e9-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="755e9-122">**詳細については、以下を参照してください**。</span><span class="sxs-lookup"><span data-stu-id="755e9-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="755e9-123">従来の電子情報開示検索と保持を Microsoft 365 コンプライアンスセンターに移行する</span><span class="sxs-lookup"><span data-stu-id="755e9-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="755e9-124">従来の電子情報開示ツールの廃止</span><span class="sxs-lookup"><span data-stu-id="755e9-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="755e9-125">インプレースの電子情報開示とインプレース保持に関する Faq</span><span class="sxs-lookup"><span data-stu-id="755e9-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



