---
title: Microsoft を指すようにドメインネームサーバーを更新する
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: b49ca9422f582f906fc6c108c85cc26150474548
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719998"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="ca8d4-102">Microsoft を指すようにドメインネームサーバーを更新する</span><span class="sxs-lookup"><span data-stu-id="ca8d4-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="ca8d4-103">注: ネーム サーバーの変更は、反映されるまで最大 48 時間かかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="ca8d4-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="ca8d4-p101">Microsoft を使用してドメインをセットアップするには、レジストラーのネームサーバーを更新する必要があります。ドメインレジストラーでネームサーバーレコードを作成または編集します。</span><span class="sxs-lookup"><span data-stu-id="ca8d4-p101">To set up your domain with Microsoft, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="ca8d4-106">ご利用のドメイン レジストラーの Web サイトにアクセスして、ネーム サーバーを編集できる領域を見つけます。</span><span class="sxs-lookup"><span data-stu-id="ca8d4-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="ca8d4-107">以下の値に一致する 2 つのネーム サーバー レコードを作成または編集します。</span><span class="sxs-lookup"><span data-stu-id="ca8d4-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="ca8d4-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="ca8d4-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="ca8d4-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="ca8d4-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="ca8d4-110">変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="ca8d4-110">Save changes.</span></span>

<span data-ttu-id="ca8d4-111">この記事の詳細な手順については、「[ネームサーバーを変更して、Microsoft 365 を任意のドメインレジストラーでセットアップする](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ca8d4-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  