---
title: 組織のグローバル アドレス一覧とオフライン アドレス帳を管理する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: a15864f34433695b61ea040abd3032d234920653
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812696"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="f3128-102">組織のグローバル アドレス一覧 (GAL) とオフライン アドレス帳 (OAB) を管理します。</span><span class="sxs-lookup"><span data-stu-id="f3128-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="f3128-103">グローバル アドレス一覧 (GAL) は、組織内のメールが有効なオブジェクト (メールを受信できるすべての受信者) の一覧です。</span><span class="sxs-lookup"><span data-stu-id="f3128-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="f3128-104">すべての組織で 1 つの GAL が自動的に作成されます。</span><span class="sxs-lookup"><span data-stu-id="f3128-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="f3128-105">追加の GAL を作成して、組織または場所ごとにユーザーを分けることができますが、1 人のユーザーが一度に表示および使用できる GAL は 1 つだけです。</span><span class="sxs-lookup"><span data-stu-id="f3128-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="f3128-106">Outlook for Windows など、一部のメール クライアントでは、オフライン用に GAL をダウンロードします。</span><span class="sxs-lookup"><span data-stu-id="f3128-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="f3128-107">これは、オフライン アドレス帳 (OAB) と呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="f3128-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="f3128-108">オンラインの Exchange では、OAB は 8 時間に 1 回のみ更新されます。クライアントはそれをダウンロードしてローカルの OAB コピーを更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f3128-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="f3128-109">受信者の変更は、最初は GAL に、その後に OAB に表示される必要があります。</span><span class="sxs-lookup"><span data-stu-id="f3128-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="f3128-110">一般的に使用されている GAL および OAB の手順をいくつか次に示します。</span><span class="sxs-lookup"><span data-stu-id="f3128-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="f3128-111">さまざまな理由から、一部のオブジェクトを GAL で非表示にしなければならない場合があります。</span><span class="sxs-lookup"><span data-stu-id="f3128-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="f3128-112">「[受信者をアドレス一覧に表示しない](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3128-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="f3128-113">特定のグループのユーザーに対してカスタマイズした組織の GAL を表示する必要がある場合は、「[Exchange Online のアドレス帳ポリシー](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3128-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="f3128-114">[Exchange Online でグローバル アドレス一覧を作成](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list)し、GAL のアクセス許可を使用する方法については、「[Exchange Online のアドレス一覧](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3128-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="f3128-115">新しい GAL を作成する場合は、新しい OAB も作成することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="f3128-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="f3128-116">「[オフライン アドレス帳の手順](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f3128-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
