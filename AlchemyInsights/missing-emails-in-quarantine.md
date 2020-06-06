---
title: 検疫に電子メールがない
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569878"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="b309d-102">検疫に電子メールがない</span><span class="sxs-lookup"><span data-stu-id="b309d-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="b309d-103">管理者は[、これらのメッセージを表示、リリース、または削除できます。](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="b309d-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="b309d-104">セキュリティ & コンプライアンスセンターを開くには、に移動 [https://protection.office.com](https://protection.office.com/) します。</span><span class="sxs-lookup"><span data-stu-id="b309d-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="b309d-105">[検疫] ページを直接開くには、に移動 [https://protection.office.com/quarantine](https://protection.office.com/quarantine) します。</span><span class="sxs-lookup"><span data-stu-id="b309d-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="b309d-106">次の値に基づいて検索できます。</span><span class="sxs-lookup"><span data-stu-id="b309d-106">You can search by the following values:</span></span>  

- <span data-ttu-id="b309d-107">**[メッセージ ID]**: メッセージのグローバル一意識別子。</span><span class="sxs-lookup"><span data-stu-id="b309d-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="b309d-108">一覧でメッセージを選択すると、表示される [**詳細**] ポップアップウィンドウに、**メッセージ ID**の値が表示されます。</span><span class="sxs-lookup"><span data-stu-id="b309d-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="b309d-109">管理者は、[メッセージ追跡](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide)を使用して、メッセージとそれに対応する [メッセージ ID] 値を検索できます。</span><span class="sxs-lookup"><span data-stu-id="b309d-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="b309d-110">**[送信者のメール アドレス]**: 単一の送信者のメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="b309d-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="b309d-111">**[受信者のメール アドレス]**: 単一の受信者のメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="b309d-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="b309d-112">**[件名]**: メッセージの件名全体を使用します。</span><span class="sxs-lookup"><span data-stu-id="b309d-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="b309d-113">この検索では大文字と小文字は区別されません。</span><span class="sxs-lookup"><span data-stu-id="b309d-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="b309d-114">検索条件を入力した後、[ ![ 更新] ボタンの [ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **更新**] をクリックして結果をフィルター処理します。  </span><span class="sxs-lookup"><span data-stu-id="b309d-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="b309d-115">検疫内のメッセージおよびファイルを表示および管理するには、次のコマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="b309d-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="b309d-116">Get-quarantinemessage を削除します。</span><span class="sxs-lookup"><span data-stu-id="b309d-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="b309d-117">Get-quarantinemessage</span><span class="sxs-lookup"><span data-stu-id="b309d-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="b309d-118">Get-quarantinemessage</span><span class="sxs-lookup"><span data-stu-id="b309d-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="b309d-119">[Get-quarantinemessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): このコマンドレットは、メッセージのみを対象としています。このコマンドレットは、SharePoint Online、OneDrive for business、または TEAMS の ATP ファイルではなく、メッセージのみを対象としています。</span><span class="sxs-lookup"><span data-stu-id="b309d-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="b309d-120">Get-quarantinemessage</span><span class="sxs-lookup"><span data-stu-id="b309d-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)