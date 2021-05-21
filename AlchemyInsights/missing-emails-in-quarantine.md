---
title: 検疫されたメールがなくなった場合
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539829"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="62ab7-102">検疫されたメールがなくなった場合</span><span class="sxs-lookup"><span data-stu-id="62ab7-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="62ab7-103">管理者は、[これらのメッセージを表示、解放、または削除](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)できます。</span><span class="sxs-lookup"><span data-stu-id="62ab7-103">Administrators can [view, release, or delete these messages.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)</span></span>

<span data-ttu-id="62ab7-104">セキュリティ/コンプライアンス センターを開くには、[https://protection.office.com](https://protection.office.com/) へ移動します。</span><span class="sxs-lookup"><span data-stu-id="62ab7-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="62ab7-105">検疫ページを直接開くには、[https://protection.office.com/quarantine](https://protection.office.com/quarantine) にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="62ab7-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="62ab7-106">次の値に基づいて検索できます。</span><span class="sxs-lookup"><span data-stu-id="62ab7-106">You can search by the following values:</span></span>  

- <span data-ttu-id="62ab7-107">**[メッセージ ID]**: メッセージのグローバル一意識別子。</span><span class="sxs-lookup"><span data-stu-id="62ab7-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="62ab7-108">一覧でメッセージを選択すると、表示される **[詳細]** ポップアップ ウィンドウに **[メッセージ ID]** 値が表示されます。</span><span class="sxs-lookup"><span data-stu-id="62ab7-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="62ab7-109">管理者は、[メッセージ追跡](/microsoft-365/security/office-365-security/message-trace-scc)を使用して、メッセージとそれに対応する [メッセージ ID] 値を検索できます。</span><span class="sxs-lookup"><span data-stu-id="62ab7-109">Admins can use [message trace](/microsoft-365/security/office-365-security/message-trace-scc) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="62ab7-110">**[送信者のメール アドレス]**: 単一の送信者のメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="62ab7-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="62ab7-111">**[受信者のメール アドレス]**: 単一の受信者のメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="62ab7-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="62ab7-112">**[件名]**: メッセージの件名全体を使用します。</span><span class="sxs-lookup"><span data-stu-id="62ab7-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="62ab7-113">この検索では大文字と小文字は区別されません。</span><span class="sxs-lookup"><span data-stu-id="62ab7-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="62ab7-114">検索条件を入力したら、![[更新] ボタン](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **[更新]** をクリックすると、結果がフィルター処理されます。</span><span class="sxs-lookup"><span data-stu-id="62ab7-114">After you've entered the search criteria, click ![Refresh button](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh** to filter the results.</span></span>

<span data-ttu-id="62ab7-115">検疫内のメッセージとファイルを表示および管理するコマンドレットは、次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="62ab7-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="62ab7-116">Delete-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="62ab7-116">Delete-QuarantineMessage</span></span>](/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="62ab7-117">Export-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="62ab7-117">Export-QuarantineMessage</span></span>](/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="62ab7-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="62ab7-118">Get-QuarantineMessage</span></span>](/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="62ab7-119">[Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): このコマンドレットはメッセージ専用であり、SharePoint Online、OneDrive for Business、Teams 用の Microsoft Defender for Office 365 からのマルウェア ファイルではないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="62ab7-119">[Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from Microsoft Defender for Office 365 for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="62ab7-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="62ab7-120">Release-QuarantineMessage</span></span>](/powershell/module/exchange/release-quarantinemessage)