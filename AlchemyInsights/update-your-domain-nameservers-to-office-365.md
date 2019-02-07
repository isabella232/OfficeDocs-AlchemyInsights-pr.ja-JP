---
title: ドメイン ネームサーバーを Office 365 に更新する
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.openlocfilehash: 244997faa41bbdefc59f8096e4c23f3f4e2d5c5e
ms.sourcegitcommit: 5dee2fcb492bd922092a6de8045a95febe57b97e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/06/2019
ms.locfileid: "29758191"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="e5ced-102">ドメイン ネームサーバーを Office 365 に更新する</span><span class="sxs-lookup"><span data-stu-id="e5ced-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="e5ced-103">注: ネーム サーバーの変更は、反映されるまで最大 48 時間かかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="e5ced-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="e5ced-p101">Office 365 でドメインを設定するには、レジストラーのネーム サーバーを更新する必要があります。ドメイン レジストラーでネーム サーバー レコードを作成または編集します。</span><span class="sxs-lookup"><span data-stu-id="e5ced-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="e5ced-106">ご利用のドメイン レジストラーの Web サイトにアクセスして、ネーム サーバーを編集できる領域を見つけます。</span><span class="sxs-lookup"><span data-stu-id="e5ced-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
    
2. <span data-ttu-id="e5ced-107">以下の値に一致する 2 つのネーム サーバー レコードを作成または編集します。</span><span class="sxs-lookup"><span data-stu-id="e5ced-107">Create or edit two nameserver records to match these values:</span></span>
    
  - <span data-ttu-id="e5ced-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="e5ced-108">ns1.bdm.microsoftonline.com</span></span>
    
  - <span data-ttu-id="e5ced-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="e5ced-109">ns2.bdm.microsoftonline.com</span></span>
    
3. <span data-ttu-id="e5ced-110">変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="e5ced-110">Save changes.</span></span>
    
<span data-ttu-id="e5ced-111">詳細な手順については、「[任意のドメイン レジストラーで Office 365 をセットアップするためにネームサーバーを変更する](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)」も参照してください。</span><span class="sxs-lookup"><span data-stu-id="e5ced-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  

