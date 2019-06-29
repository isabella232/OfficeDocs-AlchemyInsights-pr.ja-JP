---
title: 監査ログのメールボックスでの外部メール転送を識別する
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 43b6a26bc05892e71d41c4b47522785245cb4851
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383102"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="a7866-102">メールボックスで外部電子メール転送がいつ構成されたかを特定する</span><span class="sxs-lookup"><span data-stu-id="a7866-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="a7866-103">ユーザーがメールボックスで外部の電子メール転送を構成すると、アクティビティは**メールボックスの設定**コマンドレットの一部として監査されます。</span><span class="sxs-lookup"><span data-stu-id="a7866-103">When a user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="a7866-104">セキュリティ & コンプライアンスセンターで監査ログの検索を使用してアクティビティを確認できます。</span><span class="sxs-lookup"><span data-stu-id="a7866-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="a7866-105">[Office 365 セキュリティ & コンプライアンスセンター](https://protection.office.com/)にログインする</span><span class="sxs-lookup"><span data-stu-id="a7866-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="a7866-106">[**検索と調査**] をクリックして、[**監査ログの検索**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a7866-106">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="a7866-107">[**開始日**] フィールドと [**終了日**] フィールドで日付範囲を選択します。</span><span class="sxs-lookup"><span data-stu-id="a7866-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="a7866-108">ユーザー名を指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="a7866-108">You don't need to specify a username.</span></span> <span data-ttu-id="a7866-109">[**アクティビティ**] フィールドが、**すべてのアクティビティの結果を表示**するように設定されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="a7866-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="a7866-110">**[検索]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a7866-110">Click **Search**.</span></span>

<span data-ttu-id="a7866-111">結果で、[**結果のフィルター処理**] をクリックし、[アクティビティフィルター] ボックスに「 **Set-Mailbox** 」と入力します。</span><span class="sxs-lookup"><span data-stu-id="a7866-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="a7866-112">結果で監査レコードを選択します。</span><span class="sxs-lookup"><span data-stu-id="a7866-112">Select an audit record in the results.</span></span> <span data-ttu-id="a7866-113">**詳細**ポップアップで、[**詳細情報**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a7866-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="a7866-114">アクティビティが電子メール転送に関連しているかどうかを判断するには、各監査レコードの詳細を参照する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a7866-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="a7866-115">**ObjectId**: 変更されたメールボックスのエイリアス値。</span><span class="sxs-lookup"><span data-stu-id="a7866-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="a7866-116">**パラメーター**: _ForwardingSmtpAddress_は、ターゲットの電子メールアドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="a7866-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="a7866-117">**UserId**: **ObjectId**フィールドのメールボックスで電子メール転送を構成したユーザー。</span><span class="sxs-lookup"><span data-stu-id="a7866-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="a7866-118">詳細については、「[メールボックスのメール転送をセットアップするユーザーの特定](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a7866-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
