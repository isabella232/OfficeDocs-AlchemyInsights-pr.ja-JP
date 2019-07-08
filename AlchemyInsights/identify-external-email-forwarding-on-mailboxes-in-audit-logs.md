---
title: 監査ログ内のメールボックスで外部のメール転送を特定する
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
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383102"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="a9833-102">外部のメール転送がメールボックスで構成された際に、それを特定する</span><span class="sxs-lookup"><span data-stu-id="a9833-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="a9833-103">ユーザーが外部のメール転送をメールボックスで構成すると、このアクティビティは **Set-Mailbox** コマンドレットの一部として監査されます。</span><span class="sxs-lookup"><span data-stu-id="a9833-103">When a user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="a9833-104">セキュリティ/コンプライアンス センターで監査ログ検索を使用すると、アクティビティを表示できます。</span><span class="sxs-lookup"><span data-stu-id="a9833-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="a9833-105">[Office 365 セキュリティ/コンプライアンス センター](https://protection.office.com/)にログインします</span><span class="sxs-lookup"><span data-stu-id="a9833-105">[Search the audit log in the Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="a9833-106">[**検索と調査**] と [**監査ログ検索**]をクリックする。</span><span class="sxs-lookup"><span data-stu-id="a9833-106">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="a9833-107">[**開始日付**] と [**終了日付**] フィールドで日付範囲を選択します。</span><span class="sxs-lookup"><span data-stu-id="a9833-107">Select a date range using the **Start date** and **End date** fields.</span></span> <span data-ttu-id="a9833-108">ユーザー名を指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="a9833-108">You don't need to specify a value with this switch.</span></span> <span data-ttu-id="a9833-109">[**アクティビティ**] フィールドが [**すべてのアクティビティの結果を表示**] と設定されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="a9833-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="a9833-110">[**検索**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a9833-110">Click **Search**.</span></span>

<span data-ttu-id="a9833-111">結果で、[**結果をフィルター**] をクリックし、[アクティビティ] フィルター ボックスに「**Set-Mailbox**」と入力します。</span><span class="sxs-lookup"><span data-stu-id="a9833-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="a9833-112">結果で、監査レコードを選択します。</span><span class="sxs-lookup"><span data-stu-id="a9833-112">Select an audit record in the results.</span></span> <span data-ttu-id="a9833-113">[**詳細**] ポップアップから、[**詳細情報**]をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a9833-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="a9833-114">アクティビティがメールの転送に関連しているかどうかを判断するには、各監査レコードの詳細を確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a9833-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="a9833-115">**ObjectId**: 変更されたメールボックスのエイリアス値。</span><span class="sxs-lookup"><span data-stu-id="a9833-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="a9833-116">**パラメーター**: _ForwardingSmtpAddress_は、送信先のメール アドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="a9833-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="a9833-117">**UserId**: [**ObjectId**] フィールドのメールボックスでメール転送を構成したユーザー。</span><span class="sxs-lookup"><span data-stu-id="a9833-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="a9833-118">詳細については、「[メールボックスの電子メール転送を誰が設定したかを判別する](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a9833-118">Determining who set up email forwarding for a mailbox</span></span>
