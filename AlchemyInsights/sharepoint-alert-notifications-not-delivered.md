---
title: SharePoint 通知通知が配信されない
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: e682a1b3dbd0d3a1c2e52be725dd2b57fc66109a
ms.sourcegitcommit: a2c866d2f3cdc1e18a33a5b2a4209340e83ca3c2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/14/2019
ms.locfileid: "36404807"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="93b43-102">SharePoint 通知通知が配信されない</span><span class="sxs-lookup"><span data-stu-id="93b43-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="93b43-103">通知が表示される場合があるので、メールの迷惑メールフォルダーを確認してください。</span><span class="sxs-lookup"><span data-stu-id="93b43-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="93b43-104">すべての**通知が配信されていない**か、特定のファイルまたはライブラリからの**個々の通知**が配信されていないかを確認します。</span><span class="sxs-lookup"><span data-stu-id="93b43-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="93b43-105">**個別の通知が配信**されない: 特定のファイルまたはライブラリからの個々の警告が配信されない場合は、削除して再作成します。</span><span class="sxs-lookup"><span data-stu-id="93b43-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="93b43-106">通知を再作成するには、「 [SharePoint alerts を管理、表示、または削除](https://support.office.com/en-us/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=en-US&ad=US#ID0EAADAAA=Online)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="93b43-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/en-us/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=en-US&ad=US#ID0EAADAAA=Online) to recreate the alert.</span></span>
- <span data-ttu-id="93b43-107">**すべての通知が配信**されない: 複数のファイルまたはライブラリからのすべての通知が配信されない場合は、[サービス正常性ダッシュボード](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)にアクセスして、SharePoint または Exchange で発生している可能性があるすべてのアドバイザリ/インシデントをチェックします。</span><span class="sxs-lookup"><span data-stu-id="93b43-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="93b43-108">この問題は、SharePoint の通知機能または Exchange を経由した電子メールの遅延が原因である可能性があります。</span><span class="sxs-lookup"><span data-stu-id="93b43-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="93b43-109">また、他の電子メールが配信されているかどうかを確認することも重要であり、そうでない場合は、Exchange の遅延が原因であると考えられます。</span><span class="sxs-lookup"><span data-stu-id="93b43-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="93b43-110">警告の FAQ:</span><span class="sxs-lookup"><span data-stu-id="93b43-110">FAQ on alerts:</span></span>

- <span data-ttu-id="93b43-111">配布グループに通知を送信することはできません。セキュリティと O365 グループのみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="93b43-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="93b43-112">通知電子メールテンプレートをカスタマイズすることはできません。これらのことを実現するには、Microsoft FLOW または SharePoint Designer ワークフローを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="93b43-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

<span data-ttu-id="93b43-113">詳細情報:</span><span class="sxs-lookup"><span data-stu-id="93b43-113">More Information:</span></span>

- <span data-ttu-id="93b43-114">**通知のセットアップ**: 通知の設定の詳細については、「 [SharePoint でファイルまたはフォルダーが変更されたときに通知を受け取る通知を作成する](https://support.office.com/en-us/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="93b43-114">**Alert setup**: For more information about setting up alerts, see [Create an alert to get notified when a file or folder changes in SharePoint](https://support.office.com/en-us/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span></span>
- <span data-ttu-id="93b43-115">**アラートのトラブルシューティング**: 通知のトラブルシューティングの詳細については、「[ユーザーが SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/support/sites/no-alert-notifications)の通知を受信しない」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="93b43-115">**Troubleshoot alerts**: For more information about troubleshooting alerts, see [Users don't receive SharePoint Online alert notifications](https://docs.microsoft.com/en-us/sharepoint/support/sites/no-alert-notifications).</span></span>
- <span data-ttu-id="93b43-116">**Advanced O365 コンプライアンスアラートポリシー**: これらの通知の設定の詳細については、「[コンプライアンス警告ポリシー](https://docs.microsoft.com/en-us/office365/securitycompliance/alert-policies)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="93b43-116">**Advanced O365 Compliance Alert Policies**: For more information about setting up these alerts, see [Compliance Alert Policies](https://docs.microsoft.com/en-us/office365/securitycompliance/alert-policies).</span></span>
- <span data-ttu-id="93b43-117">**SharePoint および OneDrive 監査ログ**: これらのイベントを取得する方法の詳細については、「 [Search the Audit log](https://docs.microsoft.com/en-us/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="93b43-117">**SharePoint and OneDrive Audit Logs**: For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/en-us/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
- <span data-ttu-id="93b43-118">**Advanced Threat Protection によって送信されるアラート**: 「 [SharePoint および OneDrive の ATP](https://docs.microsoft.com/en-us/office365/securitycompliance/atp-for-spo-odb-and-teams)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="93b43-118">**Alerts sent by Advanced Threat Protection**: See [ATP for SharePoint and OneDrive](https://docs.microsoft.com/en-us/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
- <span data-ttu-id="93b43-119">**データ損失防止ポリシーによって送信されるアラート**: 「 [DLP ポリシーの電子メール通知](https://docs.microsoft.com/en-us/office365/securitycompliance/use-notifications-and-policy-tips)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="93b43-119">**Alerts sent by Data Loss Prevention polices**: See [Email notifications for DLP policies](https://docs.microsoft.com/en-us/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

## <a name="related-topics"></a><span data-ttu-id="93b43-120">関連項目</span><span class="sxs-lookup"><span data-stu-id="93b43-120">Related Topics</span></span>

<span data-ttu-id="93b43-121">SharePoint Online で Microsoft Flow を試す場合</span><span class="sxs-lookup"><span data-stu-id="93b43-121">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="93b43-122">フローを作成する</span><span class="sxs-lookup"><span data-stu-id="93b43-122">Create Flow</span></span>](https://support.office.com/en-us/article/create-a-flow-for-a-list-or-library-in-sharepoint-online-or-onedrive-for-business-a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="93b43-123">SharePoint およびフロー</span><span class="sxs-lookup"><span data-stu-id="93b43-123">SharePoint and Flow</span></span>](https://flow.microsoft.com/en-us/blog/sharepoint-and-flow/)
