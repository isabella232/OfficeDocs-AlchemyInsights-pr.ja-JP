---
title: IDと同じメールアドレスを持つ複数のオブジェクト
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: 05fb43133bc68b71ccdbab44d28679a1f659e762
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724620"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="18e99-102">IDと同じメールアドレスを持つ複数のオブジェクト</span><span class="sxs-lookup"><span data-stu-id="18e99-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="18e99-103">**複数のオブジェクト**</span><span class="sxs-lookup"><span data-stu-id="18e99-103">**Multiple objects**</span></span>

<span data-ttu-id="18e99-104">このエラーの一般的な理由の1つは、IDと同じ電子メールアドレスを持つ複数のオブジェクトが存在する場合に、Outlook Web Access の要求を適切にルーティングできないことです。</span><span class="sxs-lookup"><span data-stu-id="18e99-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="18e99-105">これらのオブジェクトを検索するには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="18e99-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="18e99-106">· Get-Recipient <email address></span><span class="sxs-lookup"><span data-stu-id="18e99-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="18e99-107">· Get-User <email address></span><span class="sxs-lookup"><span data-stu-id="18e99-107">· Get-User <email address></span></span>

<span data-ttu-id="18e99-108">· Get-User <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="18e99-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="18e99-109">· Get-Contact <email address></span><span class="sxs-lookup"><span data-stu-id="18e99-109">· Get-Contact <email address></span></span>

<span data-ttu-id="18e99-110">· Get-Mailbox <email address> -PublicFolder</span><span class="sxs-lookup"><span data-stu-id="18e99-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="18e99-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="18e99-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="18e99-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span><span class="sxs-lookup"><span data-stu-id="18e99-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="18e99-113">この問題を解決するには、同じメール ID を持つ複数のオブジェクトを削除し、特定のメール ID を持つオブジェクトが1つあり、その受信者タイプが UserMailbox であることを確認します。</span><span class="sxs-lookup"><span data-stu-id="18e99-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="18e99-114">**ビジネス用および個人用のメールボックスに同じアドレスが使用されている場合**</span><span class="sxs-lookup"><span data-stu-id="18e99-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="18e99-115">別の原因は、ビジネス用および個人用のメールボックスに同じアドレスが使用されている場合です。</span><span class="sxs-lookup"><span data-stu-id="18e99-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="18e99-116">この場合、Cafe がこのシナリオをサポートするまで、ユーザーはプライマリ コンシューマー エイリアスを変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="18e99-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="18e99-117">これは、介入なしでは消えない永続的なエラーです。</span><span class="sxs-lookup"><span data-stu-id="18e99-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="18e99-118">詳細については、「[Microsoft アカウントのメールアドレスまたは電話番号を変更する](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="18e99-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>