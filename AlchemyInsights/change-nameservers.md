---
title: ネームサーバを変更します。
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d011531a-0951-49c0-af30-40d2e765f381
ms.openlocfilehash: b296e76c3d39cad16f329215f0480ae260e77f2e
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28297781"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="988ce-102">ドメイン ネーム サーバーを Office 365 に更新する</span><span class="sxs-lookup"><span data-stu-id="988ce-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="988ce-103">注意: ネームサーバ変更かかる場合があります最大 48 時間に伝達します。</span><span class="sxs-lookup"><span data-stu-id="988ce-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="988ce-p101">Office 365 でドメインを設定するには、レジストラーのネーム サーバーを更新する必要があります。ドメイン レジストラーでネーム サーバー レコードを作成または編集します。</span><span class="sxs-lookup"><span data-stu-id="988ce-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="988ce-106">ドメイン レジストラーの Web サイトに移動し、ネーム サーバーを編集できる場所を見つけます。</span><span class="sxs-lookup"><span data-stu-id="988ce-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
    
2. <span data-ttu-id="988ce-107">以下の値に一致する 2 つのネーム サーバー レコードを作成または編集します。</span><span class="sxs-lookup"><span data-stu-id="988ce-107">Create or edit two nameserver records to match these values:</span></span>
    
  - <span data-ttu-id="988ce-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="988ce-108">ns1.bdm.microsoftonline.com</span></span>
    
  - <span data-ttu-id="988ce-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="988ce-109">ns2.bdm.microsoftonline.com</span></span>
    
3. <span data-ttu-id="988ce-110">変更を保存します。</span><span class="sxs-lookup"><span data-stu-id="988ce-110">Save changes.</span></span>
    
<span data-ttu-id="988ce-111">この記事でも詳細な手順を見つけることができます: [任意のドメイン レジストラーで Office 365 をセットアップするためにネームサーバーを変更する](https://support.office.com/article/https://support.office.com/en-us/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="988ce-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/https://support.office.com/en-us/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  

