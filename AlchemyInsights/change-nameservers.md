---
title: ネーム サーバーを変更する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 51532f42e7cbd39ebad3f0160465218c6e1454a2
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736654"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="55a65-102">ドメイン ネーム サーバーを Office 365 に更新する</span><span class="sxs-lookup"><span data-stu-id="55a65-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="55a65-103">注: ネーム サーバーの変更は、反映されるまで最大 48 時間かかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="55a65-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="55a65-p101">Office 365 でドメインを設定するには、レジストラーのネーム サーバーを更新する必要があります。ドメイン レジストラーでネーム サーバー レコードを作成または編集します。</span><span class="sxs-lookup"><span data-stu-id="55a65-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="55a65-106">ご利用のドメイン レジストラーの Web サイトにアクセスして、ネーム サーバーを編集できる領域を見つけます。</span><span class="sxs-lookup"><span data-stu-id="55a65-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="55a65-107">以下の値に一致する 2 つのネーム サーバー レコードを作成または編集します。</span><span class="sxs-lookup"><span data-stu-id="55a65-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="55a65-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="55a65-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="55a65-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="55a65-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="55a65-110">変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="55a65-110">Save changes.</span></span>

<span data-ttu-id="55a65-111">詳細な手順については、「[任意のドメイン レジストラーで Office 365 をセットアップするためにネームサーバーを変更する](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)」も参照してください。</span><span class="sxs-lookup"><span data-stu-id="55a65-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  