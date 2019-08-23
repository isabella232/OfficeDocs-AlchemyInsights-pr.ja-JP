---
title: メールが有効なパブリックフォルダーへのメール配信の問題を修正する
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: f7b5e5a230d26870d5e95e8762b5874f73723c6d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525118"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="9e405-102">メールが有効なパブリックフォルダーへのメール配信の問題を修正する</span><span class="sxs-lookup"><span data-stu-id="9e405-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="9e405-103">外部の送信者がメッセージをメールが有効なパブリックフォルダーに送信できず、送信者がエラーを受信できなかった場合 **(550 5.4.1)**、パブリックフォルダーの電子メールドメインが、次のような内部の中継ドメインとして構成されていることを確認します。権限のあるドメイン:</span><span class="sxs-lookup"><span data-stu-id="9e405-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="9e405-104">[Exchange 管理センター (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center)を開きます。</span><span class="sxs-lookup"><span data-stu-id="9e405-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="9e405-105">[**メールフロー** \> **承認済みドメイン**] に移動して、承認済みドメインを選択し、[**編集**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="9e405-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="9e405-106">[プロパティ] ページが開いたら、ドメインの種類が [**権限**あり] に設定されている場合は、値を [**内部の中継**] に変更し、[**保存**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="9e405-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="9e405-107">外部の送信者がアクセス許可を持っていないエラーを受け取った場合 **(550 5.7.13)**、 [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)で次のコマンドを実行して、パブリックフォルダー内の匿名ユーザーのアクセス許可を確認します。</span><span class="sxs-lookup"><span data-stu-id="9e405-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="9e405-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`たとえば、 `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`のようになります。</span><span class="sxs-lookup"><span data-stu-id="9e405-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="9e405-109">外部ユーザーがこのパブリックフォルダーに電子メールを送信できるようにするには、CreateItems アクセス権をユーザー Anonymous に追加します。</span><span class="sxs-lookup"><span data-stu-id="9e405-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="9e405-110">たとえば、`Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` などです。</span><span class="sxs-lookup"><span data-stu-id="9e405-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
