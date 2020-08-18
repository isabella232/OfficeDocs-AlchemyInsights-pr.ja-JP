---
title: SharePoint および OneDrive のアラートの受信の遅延
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 92e517ae6e83aa91b9838047ec77759dc893bc57
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/17/2020
ms.locfileid: "46785670"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="5891a-102">SharePoint および OneDrive のアラートの受信の遅延</span><span class="sxs-lookup"><span data-stu-id="5891a-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="5891a-103">まずは、メールの迷惑メール フォルダーまたはスパム フォルダーを確認します。</span><span class="sxs-lookup"><span data-stu-id="5891a-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="5891a-104">**複数のファイルまたはライブラリからのすべてのアラートの配信に遅延がある**場合は、[サービス正常性ダッシュボード](https://portal.office.com/adminportal/home?ref=/servicehealth)にアクセスして SharePoint または Exchange で発生している可能性のあるアドバイザリやインシデントを確認します。</span><span class="sxs-lookup"><span data-stu-id="5891a-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="5891a-105">問題は、SharePoint のアラート機能または Exchange を介したメールの遅延にある可能性があります。</span><span class="sxs-lookup"><span data-stu-id="5891a-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="5891a-106">また、他のメールが配信されているかどうかにも注意してください。もしも配信されていない場合には、おそらく問題は Exchange の遅延にあります。</span><span class="sxs-lookup"><span data-stu-id="5891a-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="5891a-107">**特定のファイルまたはライブラリからの個別のアラートが配信されない**場合には、削除して再作成してみてください。</span><span class="sxs-lookup"><span data-stu-id="5891a-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="5891a-108">詳細については、「[SharePoint アラートの管理、表示、または削除](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5891a-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="5891a-109">アラートを配布グループに送信することはできません。</span><span class="sxs-lookup"><span data-stu-id="5891a-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="5891a-110">セキュリティおよび O365 グループのみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="5891a-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="5891a-111">アラートのメール テンプレートをカスタマイズすることはできません。</span><span class="sxs-lookup"><span data-stu-id="5891a-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="5891a-112">これらを実現するには、Microsoft Flow または SharePoint Designer ワークフローを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5891a-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
