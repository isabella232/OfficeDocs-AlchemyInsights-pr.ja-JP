---
title: 同じメールボックスへの複数のアクティブなセッション
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1836"
- "9000248"
ms.openlocfilehash: d2fd3f20346012baed21efd4900ca4cf73391d91
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440546"
---
# <a name="multiple-active-sessions-to-the-same-mailbox"></a><span data-ttu-id="bc5cd-102">同じメールボックスへの複数のアクティブなセッション</span><span class="sxs-lookup"><span data-stu-id="bc5cd-102">Multiple active sessions to the same mailbox</span></span>

<span data-ttu-id="bc5cd-103">Exchange リソースの使用をコントロールするために、メールボックスには "予算" があります。</span><span class="sxs-lookup"><span data-stu-id="bc5cd-103">To control usage of Exchange resources, a mailbox has a "budget."</span></span>

<span data-ttu-id="bc5cd-104">予算超過の例外は、次の状況によってトリガーされますが、これに限定されません：</span><span class="sxs-lookup"><span data-stu-id="bc5cd-104">The over-budget exception can be triggered by, but is not limited to, the following circumstances:</span></span>

- <span data-ttu-id="bc5cd-105">同じ Outlook Web App セッション内でいくつかのブラウザーのタブが開かれます。　　</span><span class="sxs-lookup"><span data-stu-id="bc5cd-105">A few browser tabs are opened within the same Outlook Web App session.</span></span>

- <span data-ttu-id="bc5cd-106">同じメールボックスへのいくつかのアクティブな　Outlook Web App　セッション。</span><span class="sxs-lookup"><span data-stu-id="bc5cd-106">A few active Outlook Web App sessions to the same mailbox.</span></span>

- <span data-ttu-id="bc5cd-107">他のいくつかのクライアントアプリケーション (Outlook、Outlook Mobile、サードパーティのクライアントアプリ) は、同時にメールボックスにアクセスします。　　　</span><span class="sxs-lookup"><span data-stu-id="bc5cd-107">A few other client applications (Outlook, Outlook Mobile, a third party client app) access the mailbox at the same time.</span></span>

- <span data-ttu-id="bc5cd-108">検索要求の実行など、長時間実行される操作は、別のアクティブなメールボックスセッションから実行されます。</span><span class="sxs-lookup"><span data-stu-id="bc5cd-108">Long running operations, such as executing search requests, are performed from another active mailbox session.</span></span>

