---
title: ドメイン ステータス - サービスが選択されていません
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11094"
- "9006491"
ms.openlocfilehash: 66fae5b5602dd67954ac9208b26bc2005adda0e3
ms.sourcegitcommit: 56650eb9af437ff97e4f4d9ca5a2f53ad5bb990e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/12/2021
ms.locfileid: "53389186"
---
# <a name="domain-status---no-services-selected"></a><span data-ttu-id="aee29-102">ドメイン ステータス - サービスが選択されていません</span><span class="sxs-lookup"><span data-stu-id="aee29-102">Domain Status - No services selected</span></span>

<span data-ttu-id="aee29-103">**サービスが選択** されていないことは、Exchange Online、Skype for Business、Intune などの Microsoft 365 サービス、Microsoft 365 がカスタム ドメインで使用するモバイル デバイス管理を選択していないという意味です。</span><span class="sxs-lookup"><span data-stu-id="aee29-103">**No services selected** means you haven’t selected any Microsoft 365 services such as Exchange Online, Skype for Business or Intune, and Mobile Device Management for Microsoft 365 to use with your custom domain.</span></span> <span data-ttu-id="aee29-104">Exchange ハイブリッド (Exchange オンプレミス Exchange Online) または Exchange と他の Microsoft サービス を使用した外部スパム フィルターを使用している場合は、このメッセージを無視できます。</span><span class="sxs-lookup"><span data-stu-id="aee29-104">If you're using Exchange Hybrid (Exchange on-premises with Exchange Online) or external spam filtering with Exchange and no other Microsoft services, you can ignore this message.</span></span> <span data-ttu-id="aee29-105">ドメインの正常性状態は、サービスに直接接続されているドメインでのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="aee29-105">Domain health status is available only for domains connected directly to the service.</span></span>

<span data-ttu-id="aee29-106">ドメインのサービスを選択するには、次の方法を実行します。</span><span class="sxs-lookup"><span data-stu-id="aee29-106">To select services for your domain:</span></span>

1. <span data-ttu-id="aee29-107">**[設定** ドメイン] で、状態メッセージ [サービスなし] が選択されているドメインの横  >  [](https://admin.microsoft.com/Adminportal/Home)にあるボックス **をオンにします**。</span><span class="sxs-lookup"><span data-stu-id="aee29-107">From **Settings** > [**Domains**](https://admin.microsoft.com/Adminportal/Home), check the box next to the domain with the status message **No services selected**.</span></span>
1. <span data-ttu-id="aee29-108">[DNS **の管理] を** 選択して、ドメイン セットアップ ウィザードを開始します。</span><span class="sxs-lookup"><span data-stu-id="aee29-108">Select **Manage DNS** to start the Domain Setup Wizard.</span></span>
    - <span data-ttu-id="aee29-109">[独自の **DNS レコードを追加する] を選択した** 場合は、メッセージが表示されたら必ずサービスを選択してください。</span><span class="sxs-lookup"><span data-stu-id="aee29-109">If you choose **Add your own DNS records**, be sure to select a service when prompted.</span></span> <span data-ttu-id="aee29-110">その他のサービスは、[高度なオプション] **で利用できます**。</span><span class="sxs-lookup"><span data-stu-id="aee29-110">More services could be available under **Advanced Options**.</span></span>
    - <span data-ttu-id="aee29-111">[Microsoft に **DNS レコード** を追加する] または [その他のオプションを設定する] を選択すると、利用可能なすべてのサービスが自動的に  >  提案され、選択されます。</span><span class="sxs-lookup"><span data-stu-id="aee29-111">If you choose **Let Microsoft add your DNS records** or **More options** > **Setup my online services for me** all available services are suggested and selected automatically.</span></span>
1. <span data-ttu-id="aee29-112">ウィザードに進み、DNS セットアップとサービスの選択肢を完了します。</span><span class="sxs-lookup"><span data-stu-id="aee29-112">Continue through the wizard to complete DNS setup and your service choices.</span></span>
 
<span data-ttu-id="aee29-113">ドメインの設定に関するその他のヘルプについては、「 [ドメインに接続するための DNS レコードの追加」を参照してください](/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)。</span><span class="sxs-lookup"><span data-stu-id="aee29-113">For additional help setting up your domain, see [Add DNS records to connect your domain](/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

