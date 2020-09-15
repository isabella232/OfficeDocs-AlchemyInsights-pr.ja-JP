---
title: 組織の関係を作成して、ユーザーが他の組織と共同作業を行うことができるようにする
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
- "3800014"
- "898"
ms.openlocfilehash: a7ec7b4a8020cfe9a24d1f18af89b02400e6d45e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712738"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="acbb4-102">組織の関係を作成して、ユーザーが他の組織と共同作業を行うことができるようにする</span><span class="sxs-lookup"><span data-stu-id="acbb4-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="acbb4-103">Microsoft 365 管理センターのダッシュボードから、**[管理者]** > **[Exchange]** の順に移動します。</span><span class="sxs-lookup"><span data-stu-id="acbb4-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="acbb4-104">**[組織]** > **[共有]** の順に移動します。</span><span class="sxs-lookup"><span data-stu-id="acbb4-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="acbb4-105">**[組織の共有]** の下の **[新規作成]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="acbb4-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="acbb4-106">
            \**[組織上の関係の新規作成]** の \*\*[関係の名前]\*\* ボックスに、組織上の関係のフレンドリ名を入力します。</span><span class="sxs-lookup"><span data-stu-id="acbb4-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="acbb4-p101">**[共有するドメイン]** ボックスに、こちらの予定表を参照できるようにする外部の Office 365 または Exchange 社内組織のドメインを入力します。複数のドメインを入力する必要がある場合は、各ドメイン名をコンマで区切ります。たとえば、 contoso.com、service.contoso.com のようにします。</span><span class="sxs-lookup"><span data-stu-id="acbb4-p101">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars. If you need to enter more than one domain, separate the domain names with a comma. For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="acbb4-p102">**[予定表の空き時間情報の共有を有効にする]** チェック ボックスを選択して、指定したドメインとの予定表の共有をオンにします。予定表の空き時間情報の共有レベルと、予定表の空き時間情報を共有できるユーザーを設定します。</span><span class="sxs-lookup"><span data-stu-id="acbb4-p102">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed. Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="acbb4-112">空き時間情報のアクセス レベルを設定するには、次のいずれかを選択します。</span><span class="sxs-lookup"><span data-stu-id="acbb4-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="acbb4-113">**[時刻のみを指定して予定表の空き時間情報にアクセス]**</span><span class="sxs-lookup"><span data-stu-id="acbb4-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="acbb4-114">**[予定表の空き時間情報のうち、空き時間、件名、場所情報へのアクセス]**</span><span class="sxs-lookup"><span data-stu-id="acbb4-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="acbb4-115">予定表の空き時間情報を共有する内部ユーザーを設定するには、次のいずれかを選択します。</span><span class="sxs-lookup"><span data-stu-id="acbb4-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="acbb4-116">**組織内のすべてのユーザー**</span><span class="sxs-lookup"><span data-stu-id="acbb4-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="acbb4-117">**[指定したセキュリティ グループ]**</span><span class="sxs-lookup"><span data-stu-id="acbb4-117">**A specified security group**</span></span>  

<span data-ttu-id="acbb4-118">
            \*\*[参照]\*\* をクリックし、一覧からセキュリティ グループを選択して、\*\*[OK]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="acbb4-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="acbb4-119">
            \*\*[保存]\*\* をクリックして組織上の関係を作成します。</span><span class="sxs-lookup"><span data-stu-id="acbb4-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="acbb4-120">**注:** クロステナント構成は、空き時間情報の参照の個人用連絡先をサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="acbb4-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="acbb4-121">空き時間情報の参照を機能させるには、連絡先をグローバル アドレス一覧に含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="acbb4-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="acbb4-122">**このトピックを完全に理解するためには、以下をお読みください。**</span><span class="sxs-lookup"><span data-stu-id="acbb4-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="acbb4-123">Exchange Online で組織の関係を作成する</span><span class="sxs-lookup"><span data-stu-id="acbb4-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="acbb4-124">Exchange Online での組織の関係の変更</span><span class="sxs-lookup"><span data-stu-id="acbb4-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="acbb4-125">Exchange Online で組織の関係を削除する</span><span class="sxs-lookup"><span data-stu-id="acbb4-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
