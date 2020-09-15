---
title: メールが有効なパブリック フォルダーへの電子メール配信の問題を修正する
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677933"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="580b4-102">メールが有効なパブリック フォルダーへの電子メール配信の問題を修正する</span><span class="sxs-lookup"><span data-stu-id="580b4-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="580b4-103">外部の送信者が、メールが有効なパブリック フォルダーにメッセージを送信できないときに、送信者に **見つかりませんでした (550 5.4.1)** というエラーが示される場合は、そのパブリック フォルダーの電子メール ドメインが、権限のあるドメインではなく、内部の中継ドメインとして構成されていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="580b4-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="580b4-104">[Exchange 管理センター (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center) を開きます。</span><span class="sxs-lookup"><span data-stu-id="580b4-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="580b4-105">**[メール フロー]** \> **[承認済みドメイン]** に移動して、承認済みドメインを選択してから **[編集]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="580b4-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="580b4-106">プロパティ ページが表示されます。このページで、ドメインの種類が **[権限あり]** に設定されている場合は、その値を **[内部の中継]** に変更してから **[保存]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="580b4-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="580b4-107">外部送信者に **アクセス許可がありません (550 5.7.13)** というエラーが示される場合は、[Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) で次のコマンドを実行して、パブリック フォルダーの匿名ユーザーに対するアクセス許可を確認してください: </span><span class="sxs-lookup"><span data-stu-id="580b4-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="580b4-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`。たとえば、`Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` のようにします。</span><span class="sxs-lookup"><span data-stu-id="580b4-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="580b4-109">このパブリック フォルダーに外部ユーザーが電子メールを送信できるようにするには、ユーザー Anonymous に CreateItems アクセス権限を追加します。</span><span class="sxs-lookup"><span data-stu-id="580b4-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="580b4-110">たとえば、`Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` のようにします。</span><span class="sxs-lookup"><span data-stu-id="580b4-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
