---
title: SharePoint のアラート通知が配信されない
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
ms.openlocfilehash: f389785fcd1029ae5a47e07c723874f9f214109d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36504468"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="ffd40-102">SharePoint のアラート通知が配信されない</span><span class="sxs-lookup"><span data-stu-id="ffd40-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="ffd40-103">アラートはメールの [迷惑メール] フォルダーに移動される場合があるため、このフォルダーを確認してください。</span><span class="sxs-lookup"><span data-stu-id="ffd40-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="ffd40-104">**すべてのアラートが配信されない**のか、特定のファイルまたはライブラリからの**個別のアラートが配信されない**のかを特定します。</span><span class="sxs-lookup"><span data-stu-id="ffd40-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="ffd40-105">**個別のアラートが配信されない場合**: 特定のファイルやライブラリからの個別のアラートが配信されない場合は、アラートを削除してから再作成してみてください。</span><span class="sxs-lookup"><span data-stu-id="ffd40-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="ffd40-106">詳細については、「[SharePoint アラートの管理、表示、または削除](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=en-US&ad=US#ID0EAADAAA=Online)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ffd40-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=en-US&ad=US#ID0EAADAAA=Online) to recreate the alert.</span></span>
- <span data-ttu-id="ffd40-107">**すべてのアラートが配信されない場合**: 複数のファイルやライブラリからのすべてのアラートが配信されない場合は、[[サービス正常性](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)] ダッシュボードにアクセスして、SharePoint または Exchange でインシデントやアドバイザリが発生していないかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="ffd40-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="ffd40-108">問題の原因は、SharePoint のアラート機能によるもの、または Exchange 経由のメールの遅延によるものである可能性があります。</span><span class="sxs-lookup"><span data-stu-id="ffd40-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="ffd40-109">また、その他のメールが配信されているかどうかを確認することも重要です。配信されていない場合は、問題の原因が Exchange の遅延である可能性が高くなります。</span><span class="sxs-lookup"><span data-stu-id="ffd40-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="ffd40-110">アラートに関する FAQ:</span><span class="sxs-lookup"><span data-stu-id="ffd40-110">FAQ on alerts:</span></span>

- <span data-ttu-id="ffd40-111">配布グループにアラートを送信することはできません。サポートされているのはセキュリティ グループと O365 グループのみです。</span><span class="sxs-lookup"><span data-stu-id="ffd40-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="ffd40-112">アラート メール テンプレートをカスタマイズすることはできません。カスタマイズを行うには、Microsoft FLOW または SharePoint Designer ワークフローを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ffd40-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

<span data-ttu-id="ffd40-113">詳細情報:</span><span class="sxs-lookup"><span data-stu-id="ffd40-113">More information</span></span>

- <span data-ttu-id="ffd40-114">**アラートの設定**: アラートの設定の詳細については、「[SharePoint でファイルやフォルダーが変更されたときに知らせてくれる通知を作成する](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ffd40-114">**Alert setup**: For more information about setting up alerts, see [Create an alert to get notified when a file or folder changes in SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span></span>
- <span data-ttu-id="ffd40-115">**アラートのトラブルシューティング**: アラートのトラブルシューティングの詳細については、「[ユーザーが SharePoint Online アラート通知を受信していない](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ffd40-115">**Troubleshoot alerts**: For more information about troubleshooting alerts, see [Users don't receive SharePoint Online alert notifications](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).</span></span>
- <span data-ttu-id="ffd40-116">**高度な O365 コンプライアンス アラート ポリシー**: この種類のアラートの設定の詳細については、「[コンプライアンス アラート ポリシー](https://docs.microsoft.com/office365/securitycompliance/alert-policies)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ffd40-116">**Advanced O365 Compliance Alert Policies**: For more information about setting up these alerts, see [Compliance Alert Policies](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span></span>
- <span data-ttu-id="ffd40-117">**SharePoint および OneDrive 監査ログ**: これらのイベントを取得する方法の詳細については、「[監査ログを検索する](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ffd40-117">**SharePoint and OneDrive Audit Logs**: For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
- <span data-ttu-id="ffd40-118">**Advanced Threat Protection によって送信されるアラート**: 「[ATP for SharePoint and OneDrive (SharePoint および OneDrive 用の ATP)](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ffd40-118">**Alerts sent by Advanced Threat Protection**: See [ATP for SharePoint and OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
- <span data-ttu-id="ffd40-119">**データ損失防止ポリシーによって送信されるアラート**: 「[Email notifications for DLP policies (DLP ポリシーのメール通知)](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ffd40-119">**Alerts sent by Data Loss Prevention polices**: See [Email notifications for DLP policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

## <a name="related-topics"></a><span data-ttu-id="ffd40-120">関連項目</span><span class="sxs-lookup"><span data-stu-id="ffd40-120">Related Topics</span></span>

<span data-ttu-id="ffd40-121">SharePoint Online で Microsoft Flow を試す方法。</span><span class="sxs-lookup"><span data-stu-id="ffd40-121">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="ffd40-122">フローを作成する</span><span class="sxs-lookup"><span data-stu-id="ffd40-122">Create Flow</span></span>](https://support.office.com/article/create-a-flow-for-a-list-or-library-in-sharepoint-online-or-onedrive-for-business-a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="ffd40-123">SharePoint and Flow (SharePoint と Flow)</span><span class="sxs-lookup"><span data-stu-id="ffd40-123">SharePoint and Flow</span></span>](https://flow.microsoft.com/en-us/blog/sharepoint-and-flow/)
