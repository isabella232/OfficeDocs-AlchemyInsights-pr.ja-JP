---
title: Outlook for Windows で代理人を追加または削除する方法
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573948"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a><span data-ttu-id="18ab5-102">Outlook for Windows で代理人を追加または削除する方法</span><span class="sxs-lookup"><span data-stu-id="18ab5-102">How to add or remove a Delegate in Outlook for Windows</span></span>

<span data-ttu-id="18ab5-103">Outlook for Windows で代理人を追加するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="18ab5-103">To add a Delegate in Outlook for Windows:</span></span> 

1. <span data-ttu-id="18ab5-104">[**ファイル**] タブをクリックし、[**アカウント設定**] をクリックしてから、[**代理人アクセス**] を選びます。</span><span class="sxs-lookup"><span data-stu-id="18ab5-104">Click on the **File** tab followed by **Account Settings**, and then choose **Delegate Access**.</span></span>
2. <span data-ttu-id="18ab5-105">[**追加**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="18ab5-105">Click on **Add**.</span></span> <span data-ttu-id="18ab5-106">[**追加**] が表示されない場合は、Outlook と Exchange が接続されていない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="18ab5-106">If **Add** doesn’t appear, an active connection might not exist between Outlook and Exchange.</span></span> <span data-ttu-id="18ab5-107">Outlook のステータス バーに接続状態が表示されます。</span><span class="sxs-lookup"><span data-stu-id="18ab5-107">The Outlook status bar displays the connection status.</span></span>
3. <span data-ttu-id="18ab5-108">代理人に指定する人の名前を入力するか、または検索して検索結果の一覧から名前を選びます。</span><span class="sxs-lookup"><span data-stu-id="18ab5-108">Type the name of the person you want to designate as your delegate, or search and choose the name in the search results list.</span></span>

    > [!NOTE]
    > <span data-ttu-id="18ab5-109">代理人は、組織の Exchange のグローバル アドレス一覧 (GAL) に含まれているユーザーである必要があります。</span><span class="sxs-lookup"><span data-stu-id="18ab5-109">The delegate must be a person in your organization's Exchange Global Address List (GAL).</span></span>
4. <span data-ttu-id="18ab5-110">[**追加**] をクリックし、[**OK**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="18ab5-110">Click on **Add** followed by **OK**.</span></span>
5. <span data-ttu-id="18ab5-111">[**代理アクセス権の設定**] ダイアログ ボックスで、既定のアクセス権設定を使用するか、または Exchange フォルダーに対するユーザー設定のアクセス レベルを選択できます。</span><span class="sxs-lookup"><span data-stu-id="18ab5-111">In the **Delegate Permissions** dialog box, accept the default permission settings or select custom access levels for Exchange folders.</span></span>

    - <span data-ttu-id="18ab5-112">代理人に会議出席依頼と返信の操作だけを許可するのであれば、[**会議関係のメールを代理人にも送信する**] などの既定のアクセス権設定で十分です。</span><span class="sxs-lookup"><span data-stu-id="18ab5-112">If a delegate needs permission to work only with meeting requests and responses, the default permission settings such as **Delegate receives copies of meeting-related messages sent to me** are sufficient.</span></span> <span data-ttu-id="18ab5-113">**受信トレイ** へのアクセス権は [**なし**] にしておくことができます。</span><span class="sxs-lookup"><span data-stu-id="18ab5-113">You can leave the **Inbox** permission setting at **None**.</span></span> <span data-ttu-id="18ab5-114">会議出席依頼と返答は、代理人の受信トレイに直接配信されます。</span><span class="sxs-lookup"><span data-stu-id="18ab5-114">Meeting requests and responses will go directly to the delegate's inbox.</span></span>

    > [!NOTE]
    > <span data-ttu-id="18ab5-115">既定では、代理人に委任者の [**予定表**] フォルダーへの [**編集者 (アイテムを参照、作成、変更できる)**] アクセス権が付与されます。</span><span class="sxs-lookup"><span data-stu-id="18ab5-115">By default, the delegate is granted **Editor (can read, create, and modify items)** permission to your **Calendar** folder.</span></span> <span data-ttu-id="18ab5-116">代理人が代わりに会議出席依頼に返信すると、委任者の [**予定表**] フォルダーに会議が自動的に追加されます。</span><span class="sxs-lookup"><span data-stu-id="18ab5-116">When the delegate responds to a meeting on your behalf, it is automatically added to your **Calendar** folder.</span></span>

5. <span data-ttu-id="18ab5-117">権限が変更されたことを通知するメッセージを代理人に送信するには、[**設定したアクセス権情報を代理人に自動送信する**] チェック ボックスをオンにします。</span><span class="sxs-lookup"><span data-stu-id="18ab5-117">To send a message to notify the delegate of the changed permissions, select the **Automatically send a message to delegate summarizing these permissions** check box.</span></span>
6. <span data-ttu-id="18ab5-118">必要に応じて、[**代理人に非公開に設定したアイテムへのアクセスを許可する**] チェック ボックスをオンにします。</span><span class="sxs-lookup"><span data-stu-id="18ab5-118">If you want, select the **Delegate can see my private items** check box.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="18ab5-119">この設定はすべての Exchange フォルダーに適用されます。</span><span class="sxs-lookup"><span data-stu-id="18ab5-119">This setting affects all Exchange folders.</span></span> <span data-ttu-id="18ab5-120">[メール]、[連絡先]、[予定表]、[タスク]、[メモ]、[履歴] など、すべてのフォルダーの非公開アイテムへのアクセスが許可されます。</span><span class="sxs-lookup"><span data-stu-id="18ab5-120">This includes all Mail, Contacts, Calendar, Tasks, Notes, and Journal folders.</span></span> <span data-ttu-id="18ab5-121">特定のフォルダーに対してのみ非公開アイテムへのアクセスを許可することはできません。</span><span class="sxs-lookup"><span data-stu-id="18ab5-121">There is no way to grant access to private items in only specified folders.</span></span>

7. <span data-ttu-id="18ab5-122">[**OK**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="18ab5-122">Choose **OK**.</span></span>

    > [!NOTE]
    >
    > - <span data-ttu-id="18ab5-123">代理送信アクセス権で送信されたメッセージは、[**差出人**] に代理人と委任者の両方の名前が表示されます。</span><span class="sxs-lookup"><span data-stu-id="18ab5-123">Messages sent with Send on Behalf permissions include both the delegate's and your names next to **From**.</span></span> <span data-ttu-id="18ab5-124">送信者アクセス権で送信されたメッセージには、委任者の名前だけが表示されます。</span><span class="sxs-lookup"><span data-stu-id="18ab5-124">When a message is sent with Send As permissions, only your name appears.</span></span>
    > - <span data-ttu-id="18ab5-125">代理人のユーザーを追加すると、そのユーザーの Outlook プロファイルに Exchange メールボックスを追加できます。</span><span class="sxs-lookup"><span data-stu-id="18ab5-125">Once you add someone as a delegate, they can add your Exchange mailbox to their Outlook profile.</span></span> <span data-ttu-id="18ab5-126">詳細な方法については、「[他のユーザーのメールおよび予定表のアイテムを管理する](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="18ab5-126">For instructions, see [Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span></span>

<span data-ttu-id="18ab5-127">Outlook for Windows で代理人を削除するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="18ab5-127">To remove a Delegate in Outlook for Windows:</span></span>

1. <span data-ttu-id="18ab5-128">[**ファイル**] タブをクリックします。</span><span class="sxs-lookup"><span data-stu-id="18ab5-128">Click on the **File** tab.</span></span>
2. <span data-ttu-id="18ab5-129">[**アカウント設定**] をクリックし、[**代理人アクセス**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="18ab5-129">Click on **Account Settings** followed by **Delegate Access**.</span></span>
3. <span data-ttu-id="18ab5-130">アクセス権を変更する代理人の名前を選んで、[**削除**] をクリックし、[**OK**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="18ab5-130">Choose the name of the delegate for whom you want to change permissions, and then click on **Remove** followed by **OK**.</span></span>
