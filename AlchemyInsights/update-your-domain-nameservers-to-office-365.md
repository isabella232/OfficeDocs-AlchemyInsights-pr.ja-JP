---
title: ドメイン ネームサーバーを Office 365 に更新する
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 23d49c734148739ede0d5e5b53430a42b606c831
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/18/2019
ms.locfileid: "36742185"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="c773b-102">ドメイン ネームサーバーを Office 365 に更新する</span><span class="sxs-lookup"><span data-stu-id="c773b-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="c773b-103">注: ネーム サーバーの変更は、反映されるまで最大 48 時間かかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="c773b-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="c773b-p101">Office 365 でドメインを設定するには、レジストラーのネーム サーバーを更新する必要があります。ドメイン レジストラーでネーム サーバー レコードを作成または編集します。</span><span class="sxs-lookup"><span data-stu-id="c773b-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="c773b-106">ご利用のドメイン レジストラーの Web サイトにアクセスして、ネーム サーバーを編集できる領域を見つけます。</span><span class="sxs-lookup"><span data-stu-id="c773b-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="c773b-107">以下の値に一致する 2 つのネーム サーバー レコードを作成または編集します。</span><span class="sxs-lookup"><span data-stu-id="c773b-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="c773b-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="c773b-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="c773b-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="c773b-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="c773b-110">変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="c773b-110">Save changes.</span></span>

<span data-ttu-id="c773b-111">詳細な手順については、「[任意のドメイン レジストラーで Office 365 をセットアップするためにネームサーバーを変更する](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)」も参照してください。</span><span class="sxs-lookup"><span data-stu-id="c773b-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  