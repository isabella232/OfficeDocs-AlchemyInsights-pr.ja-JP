---
title: 着信メールに返信するためのルールを設定する
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "7254"
ms.openlocfilehash: 49b8aafe77aa6e31f8d724046c6fc0996294cc5d
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527804"
---
# <a name="set-up-rules-to-reply-to-incoming-emails"></a><span data-ttu-id="7fe98-102">着信メールに返信するためのルールを設定する</span><span class="sxs-lookup"><span data-stu-id="7fe98-102">Set up rules to reply to incoming emails</span></span>

<span data-ttu-id="7fe98-103">以下の手順を使ってメッセージに応答するテンプレートを作成し、受け取ったすべてのメッセージに応答するように Outlook を設定します。</span><span class="sxs-lookup"><span data-stu-id="7fe98-103">Use the following steps to create a template to reply to messages, and then set up Outlook to reply to every message you receive.</span></span>

1. <span data-ttu-id="7fe98-104">Outlook で新しいメール メッセージを作成し、不在時テンプレートの件名とメッセージ本文を入力します。</span><span class="sxs-lookup"><span data-stu-id="7fe98-104">In Outlook, create a new email message and enter a subject and message body for your out-of-office template.</span></span>
2. <span data-ttu-id="7fe98-105">**[ファイル]、[名前を付けて保存]** の順に選びます。</span><span class="sxs-lookup"><span data-stu-id="7fe98-105">Select **File > Save As**.</span></span>
3. <span data-ttu-id="7fe98-106">**[名前を付けて保存]** ダイアログ ボックスから、**[ファイルの種類]** ドロップダウンで **[Outlook テンプレート (\*.oft)]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="7fe98-106">In the **Save As** dialog box, from the **Save as type** drop-down, select **Outlook Template (\*.oft).**</span></span> <span data-ttu-id="7fe98-107">適切な名前を付けてから、**[保存]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="7fe98-107">Give it an appropriate name, and then click **Save**.</span></span>
4. <span data-ttu-id="7fe98-108">**[ファイル]** > **[仕分けルールと通知の管理]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="7fe98-108">Select the **File** > **Manage Rules & Alerts**.</span></span>
5. <span data-ttu-id="7fe98-109">**[仕分けルールと通知]** ダイアログ ボックスの **[電子メールの仕分けルール]** タブで、**[新しい仕分けルール]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="7fe98-109">In the **Rules and Alerts** dialog box, on the **E-mail Rules** tab, click **New Rule**.</span></span>
6. <span data-ttu-id="7fe98-110">**[自動仕分けウィザード]** ダイアログ ボックスで、**[新しい仕分けルールを作成する]** の **[受信メッセージにルールを適用する]** をクリックし、**[次へ]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="7fe98-110">In the **Rules Wizard** dialog box, under **Start from a blank rule**, select **Apply rule on messages I receive**, and then click **Next**.</span></span>
7. <span data-ttu-id="7fe98-111">条件として、**[自分だけに送信された場合]** を選択し、**[次へ]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="7fe98-111">For the condition, select **sent only to me**, and then click **Next**.</span></span>
8. <span data-ttu-id="7fe98-112">操作として、**[特定のテンプレートを使用して返信]** を選択し、下部のウィンドウで **[特定のテンプレート]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="7fe98-112">For the action, select **reply using a specific template**, and then in the bottom pane, click **a specific template**.</span></span>
9. <span data-ttu-id="7fe98-113">**[返信用テンプレートの選択]** ダイアログ ボックスで、**[フォルダーの場所]** ドロップダウンから **[ファイル システム内のユーザー テンプレート]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="7fe98-113">In the **Select a Reply Template** dialog box, from the **Look In** drop-down, select **User Templates in File System**.</span></span> <span data-ttu-id="7fe98-114">前に保存したテンプレートを選択し、**[開く]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="7fe98-114">Choose the previously saved template, and then click **Open**.</span></span>
10. <span data-ttu-id="7fe98-115">ダイアログボックスの下部ウィンドウに、テンプレート ファイルが挿入されていることが表示されます。</span><span class="sxs-lookup"><span data-stu-id="7fe98-115">In the bottom pane of the dialog box you'll see that the template file is inserted.</span></span> <span data-ttu-id="7fe98-116">**[終了]** をクリックしてウィザードを閉じ、**[仕分けルールと通知]** ダイアログ ボックスに戻ります。</span><span class="sxs-lookup"><span data-stu-id="7fe98-116">Click **Finish** to close the wizard and return to the **Rules and Alerts** dialog box.</span></span> <span data-ttu-id="7fe98-117">新しく作成された **[自分だけに送信された場合]** ルールに注意してください。</span><span class="sxs-lookup"><span data-stu-id="7fe98-117">Notice the newly created **sent only to me** rule.</span></span> <span data-ttu-id="7fe98-118">**[OK]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="7fe98-118">Click **OK**.</span></span>
