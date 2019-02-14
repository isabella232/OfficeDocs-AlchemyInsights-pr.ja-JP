---
title: ネーム サーバーを変更する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d011531a-0951-49c0-af30-40d2e765f381
ms.openlocfilehash: 1b49321d3bcc066136080da09be6d534ec3c3bbb
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "29912827"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="6b8d2-102">ドメイン ネーム サーバーを Office 365 に更新する</span><span class="sxs-lookup"><span data-stu-id="6b8d2-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="6b8d2-103">注: ネーム サーバーの変更は、反映されるまで最大 48 時間かかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="6b8d2-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="6b8d2-p101">Office 365 でドメインを設定するには、レジストラーのネーム サーバーを更新する必要があります。ドメイン レジストラーでネーム サーバー レコードを作成または編集します。</span><span class="sxs-lookup"><span data-stu-id="6b8d2-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="6b8d2-106">ご利用のドメイン レジストラーの Web サイトにアクセスして、ネーム サーバーを編集できる領域を見つけます。</span><span class="sxs-lookup"><span data-stu-id="6b8d2-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
    
2. <span data-ttu-id="6b8d2-107">以下の値に一致する 2 つのネーム サーバー レコードを作成または編集します。</span><span class="sxs-lookup"><span data-stu-id="6b8d2-107">Create or edit two nameserver records to match these values:</span></span>
    
  - <span data-ttu-id="6b8d2-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="6b8d2-108">ns1.bdm.microsoftonline.com</span></span>
    
  - <span data-ttu-id="6b8d2-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="6b8d2-109">ns2.bdm.microsoftonline.com</span></span>
    
3. <span data-ttu-id="6b8d2-110">変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="6b8d2-110">Save changes.</span></span>
    
<span data-ttu-id="6b8d2-111">詳細な手順については、「[任意のドメイン レジストラーで Office 365 をセットアップするためにネームサーバーを変更する](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)」も参照してください。</span><span class="sxs-lookup"><span data-stu-id="6b8d2-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  

