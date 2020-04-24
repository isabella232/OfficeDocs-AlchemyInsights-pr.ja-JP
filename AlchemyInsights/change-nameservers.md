---
title: ネーム サーバーを変更する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 572f8befd84f55cb07a3535852a46e735d3ed620
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706760"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="23fe0-102">Microsoft を指すようにドメイン ネームサーバーを更新する</span><span class="sxs-lookup"><span data-stu-id="23fe0-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="23fe0-103">注: ネーム サーバーの変更は、反映されるまで最大 48 時間かかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="23fe0-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="23fe0-p101">Microsoft 365 でドメインを設定するには、レジストラーのネーム サーバーを更新する必要があります。ドメイン レジストラーでネーム サーバー レコードを作成または編集します。</span><span class="sxs-lookup"><span data-stu-id="23fe0-p101">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="23fe0-106">ご利用のドメイン レジストラーの Web サイトにアクセスして、ネーム サーバーを編集できる領域を見つけます。</span><span class="sxs-lookup"><span data-stu-id="23fe0-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="23fe0-107">以下の値に一致する 2 つのネーム サーバー レコードを作成または編集します。</span><span class="sxs-lookup"><span data-stu-id="23fe0-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="23fe0-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="23fe0-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="23fe0-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="23fe0-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="23fe0-110">変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="23fe0-110">Save changes.</span></span>

<span data-ttu-id="23fe0-111">詳細な手順については、「[任意のドメイン レジストラーでネームサーバーを変更する](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)」も参照してください。</span><span class="sxs-lookup"><span data-stu-id="23fe0-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  