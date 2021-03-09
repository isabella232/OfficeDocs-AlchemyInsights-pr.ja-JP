---
title: DKIM レコードの書式設定に関する一般的な問題を修正する
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527827"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a><span data-ttu-id="85589-102">DKIM レコードの書式設定に関する一般的な問題を修正する</span><span class="sxs-lookup"><span data-stu-id="85589-102">Fix common problems with DKIM record formatting</span></span>

<span data-ttu-id="85589-103">ほとんどの DKIM セットアップの問題は、不適切な DNS レコードに関連しています。</span><span class="sxs-lookup"><span data-stu-id="85589-103">Most DKIM set-up issues are related to incorrect DNS records.</span></span>

<span data-ttu-id="85589-104">DKIM セットアップの問題を修正するには、DKIM CNAME レコード (TXT レコード **ではありません**) の書式が正しいことを確認します。</span><span class="sxs-lookup"><span data-stu-id="85589-104">To fix the DKIM set-up issues, verify that the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="85589-105">詳細については、「[Office 365 で DKIM を手動でセットアップする手順](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="85589-105">For more information, see [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span></span>

<span data-ttu-id="85589-106">DNS レコード全般についてサポートが必要な場合は、「[任意の DNS ホスティング プロバイダーで Office 365 用に DNS レコードを作成する](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="85589-106">If you need help with DNS records in general, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

> [!NOTE]
> <span data-ttu-id="85589-107">ドメインの DNS ホスティン グサービスで DKIM DNS レコードを作成または更新したら、その DNS レコードが伝達されるまで待機する必要があります。</span><span class="sxs-lookup"><span data-stu-id="85589-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain, you'll need to wait for the DNS records to propagate.</span></span>
