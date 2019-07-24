---
title: SharePoint のアラート通知が配信されない
ms.author: efrene
author: efrene
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 65c9c31a0dfb49c636b719b27edd04428914a88d
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840593"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="f982b-102">SharePoint のアラート通知が配信されない</span><span class="sxs-lookup"><span data-stu-id="f982b-102">SharePoint alert notifications not delivered</span></span> 

<span data-ttu-id="f982b-103">まず、すべてのアラートが配信されなくなっているのか、特定のファイルまたはライブラリからの個別のアラートが配信されなくなっているのかを調べてください。</span><span class="sxs-lookup"><span data-stu-id="f982b-103">First, determine if all alerts are not delivered or if an individual alert from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="f982b-104">**すべてのアラートが配信されない場合**: 複数のファイルやライブラリからのすべてのアラートが配信されない場合は、[[サービス正常性](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)] ダッシュボードにアクセスして、SharePoint または Exchange で発生している可能性のあるインシデントやアドバイザリを確認します。</span><span class="sxs-lookup"><span data-stu-id="f982b-104">**All alerts are not delivered**:  If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="f982b-105">問題の原因は、SharePoint のアラート機能によるもの、または Exchange 経由のメールの遅延によるものである可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f982b-105">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="f982b-106">また、その他のメールが配信されているかどうかを確認することも重要です。配信されていない場合は、問題の原因が Exchange の遅延である可能性が高くなります。</span><span class="sxs-lookup"><span data-stu-id="f982b-106">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span> 

- <span data-ttu-id="f982b-107">**個別のアラートが配信されない場合**: 特定のファイルやライブラリからの個別のアラートが配信されない場合は、アラートを削除してから再作成してみてください。</span><span class="sxs-lookup"><span data-stu-id="f982b-107">**Individual alerts are not delivered**:  If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="f982b-108">「[SharePoint アラートの管理、表示、または削除</a>」を参照して、アラートを再作成します](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2#ID0EAADAAA=Online)。</span><span class="sxs-lookup"><span data-stu-id="f982b-108">See [Manage, view, or delete SharePoint alerts</a> to recreate the alert](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2#ID0EAADAAA=Online).</span></span> 
 
<span data-ttu-id="f982b-109">警告に関する関連情報:</span><span class="sxs-lookup"><span data-stu-id="f982b-109">More about alerts:</span></span>

- <span data-ttu-id="f982b-110">**アラートの設定**: アラートの設定の詳細については、「[SharePoint でファイルやフォルダーが変更されたときに知らせてくれる通知を作成する](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f982b-110">**Alert setup**: For more information about setting up alerts, see [Create an alert to get notified when a file or folder changes in SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span></span>

- <span data-ttu-id="f982b-111">**アラートのトラブルシューティング**: アラートのトラブルシューティングの詳細については、「[ユーザーが SharePoint Online アラート通知を受信していない](https://support.office.com/article/users-don-t-receive-sharepoint-online-alert-notifications-14fc22dd-e873-482c-844d-f67ad41313f1)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f982b-111">**Troubleshoot alerts**:  For more information about troubleshooting alerts, see [Users don't receive SharePoint Online alert notifications](https://support.office.com/article/users-don-t-receive-sharepoint-online-alert-notifications-14fc22dd-e873-482c-844d-f67ad41313f1).</span></span>



