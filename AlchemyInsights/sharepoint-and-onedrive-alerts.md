---
title: SharePoint および OneDrive のアラートの受信の遅延
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: e5476f4e8462f233ff2a46832742d5a1f6e14e73
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599857"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="c256d-102">SharePoint および OneDrive のアラートの受信の遅延</span><span class="sxs-lookup"><span data-stu-id="c256d-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="c256d-103">**複数のファイルまたはライブラリからのすべてのアラートの配信に遅延がある** 場合は、[ サービス正常性ダッシュボード](https://portal.office.com/adminportal/home?ref=/servicehealth) にアクセスして SharePoint または Exchange で発生している可能性のあるアドバイザリやインシデントを確認します。</span><span class="sxs-lookup"><span data-stu-id="c256d-103">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span>
- <span data-ttu-id="c256d-104">**特定のファイルまたはライブラリからの個別のアラートが配信されない** 場合には、削除して再作成してみてください。</span><span class="sxs-lookup"><span data-stu-id="c256d-104">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="c256d-105">詳細については、「[ SharePoint アラートの管理、表示、または削除 ](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) 」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c256d-105">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>
- <span data-ttu-id="c256d-106">まずは、メールの迷惑メール フォルダーまたはスパム フォルダーを確認します。</span><span class="sxs-lookup"><span data-stu-id="c256d-106">Check the Junk or Spam folder in your email.</span></span>

> [!NOTE]
> - <span data-ttu-id="c256d-107">アラートを配布グループに送信することはできません。</span><span class="sxs-lookup"><span data-stu-id="c256d-107">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="c256d-108">セキュリティおよび O365 グループのみがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="c256d-108">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="c256d-109">アラートのメール テンプレートをカスタマイズすることはできません。</span><span class="sxs-lookup"><span data-stu-id="c256d-109">You cannot customize alert email templates.</span></span> <span data-ttu-id="c256d-110">これらを実現するには、Microsoft Flow または SharePoint Designer ワークフローを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c256d-110">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
