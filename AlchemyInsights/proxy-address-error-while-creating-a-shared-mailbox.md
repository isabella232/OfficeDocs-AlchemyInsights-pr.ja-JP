---
title: 共有メールボックスの作成時に発生するプロキシ アドレス エラー
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568295"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a><span data-ttu-id="b61eb-102">メールボックスまたはメールが有効なその他のオブジェクトの作成時に発生するプロキシ アドレス エラー</span><span class="sxs-lookup"><span data-stu-id="b61eb-102">Proxy address error while creating a mailbox or other email enabled object</span></span>

<span data-ttu-id="b61eb-103">メールが有効なオブジェクト (メールボックス、共有メールボックスなど) を作成しようとしたところ、「プロキシ アドレス "SMTP:alias@domain.com" は既に使用されています...」というエラーが表示される場合は、選択したメール アドレスが組織内のメールが有効な別のオブジェクトで既に使用されています。</span><span class="sxs-lookup"><span data-stu-id="b61eb-103">If you tried to create an email-enabled object (mailbox, shared mailbox etc.) and received the error "The proxy address "SMTP:alias@domain.com" is already being used…", the email address you chose is already taken by another email-enabled object in your organization.</span></span>
  
<span data-ttu-id="b61eb-104">このメール アドレスが指定されているユーザー、グループ、共有メールボックス、またはパブリック フォルダーを検索して、削除するか、メール アドレスを変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b61eb-104">You need to find the user, group, shared mailbox or public folder that has this email address and delete it or change its email address.</span></span> <span data-ttu-id="b61eb-105">その後、解放されたメール アドレスを使用してメールが有効なオブジェクトを新しく作成できるようになります。</span><span class="sxs-lookup"><span data-stu-id="b61eb-105">Then you can create a new email-enabled object with the freed email address.</span></span> <span data-ttu-id="b61eb-106">メール アドレスを検索するには、ホームページの [検索] を使用します。</span><span class="sxs-lookup"><span data-stu-id="b61eb-106">Use Search on the Home page to find it.</span></span> <span data-ttu-id="b61eb-107">次の Exchange Online PowerShell コマンドを使って検索することもできます。</span><span class="sxs-lookup"><span data-stu-id="b61eb-107">You can also use the following Exchange Online PowerShell command to search for it:</span></span>

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
<span data-ttu-id="b61eb-108">既存のメール アドレスを削除しない場合は、作成しようとしている新しいオブジェクトに対して新しいメール アドレスを選択します。</span><span class="sxs-lookup"><span data-stu-id="b61eb-108">If you don't want to delete the existing email address, choose a new email address for the new object you are creating.</span></span>
  