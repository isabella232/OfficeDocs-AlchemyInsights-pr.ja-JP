---
title: IMAP からメールを移行する
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom:
- "732"
- "1200030"
ms.assetid: 1d51fc10-cb67-4afa-a597-aef8dc90b9f8
ms.openlocfilehash: e59912d98125002cf97a6b4a5201c2c73421c98f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47754848"
---
# <a name="when-you-get-a-not-an-accepted-domain-error"></a><span data-ttu-id="5bd45-102">「承認済みドメインではありません」というエラーが表示される場合</span><span class="sxs-lookup"><span data-stu-id="5bd45-102">When you get a "Not an accepted domain" error</span></span>

<span data-ttu-id="5bd45-103">ユーザーまたはグループにメール アドレスを追加するとき、または Microsoft 365 メールボックスの移行中に、[**ドメインは、まだ Exchange システムの承認済みドメインではないため、使うことができません。**] というエラーが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5bd45-103">When trying to add an email address on the user or a group or during migration of Microsoft 365 mailboxes, you might be getting the following error: **You can't use the domain because it's not an accepted domain for Exchange System yet.**</span></span>
  
<span data-ttu-id="5bd45-104">多くの場合、このエラーはドメイン名 *(contoso.com など)* がお客様の組織用に完全に設定されていないために発生します。</span><span class="sxs-lookup"><span data-stu-id="5bd45-104">In most cases, this error is a result of the domain name *(such as contoso.com)*  not being fully set up for your organization.</span></span>
  
<span data-ttu-id="5bd45-105">「[Microsoft 365 へのドメインの追加](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain)」の手順に従って、ドメインが完全に設定されていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="5bd45-105">Please verify that the domain is fully setup by following the instructions in [Add a domain to Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/setup/add-domain).</span></span>
  