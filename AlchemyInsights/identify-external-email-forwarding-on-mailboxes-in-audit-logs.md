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
ms.openlocfilehash: 7defd0902e8c8bebae9c7bfee72c3199cbc1909f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539106"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="cb1ee-102">メールボックスで外部電子メール転送がいつ構成されたかを特定する</span><span class="sxs-lookup"><span data-stu-id="cb1ee-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="cb1ee-103">Office 365 ユーザーがメールボックスで外部の電子メール転送を構成する場合、アクティビティは**メールボックスの設定**コマンドレットの一部として監査されます。</span><span class="sxs-lookup"><span data-stu-id="cb1ee-103">When an Office 365  user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="cb1ee-104">セキュリティ & コンプライアンスセンターで監査ログの検索を使用してアクティビティを確認できます。</span><span class="sxs-lookup"><span data-stu-id="cb1ee-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="cb1ee-105">[Office 365 セキュリティ & コンプライアンスセンター](https://protection.office.com/)にログインします。</span><span class="sxs-lookup"><span data-stu-id="cb1ee-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="cb1ee-106">[ \*\*\*\* > **監査ログ**の検索] ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="cb1ee-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="cb1ee-107">[**開始日**] フィールドと [**終了日**] フィールドで日付範囲を選択します。</span><span class="sxs-lookup"><span data-stu-id="cb1ee-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="cb1ee-108">ユーザー名を指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="cb1ee-108">You don't need to specify a username.</span></span> <span data-ttu-id="cb1ee-109">[**アクティビティ**] フィールドが、**すべてのアクティビティの結果を表示**するように設定されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="cb1ee-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="cb1ee-110">**[検索]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="cb1ee-110">Click **Search**.</span></span>

<span data-ttu-id="cb1ee-111">結果で、[**結果のフィルター処理**] をクリックし、[アクティビティフィルター] ボックスに「 **Set-Mailbox** 」と入力します。</span><span class="sxs-lookup"><span data-stu-id="cb1ee-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="cb1ee-112">結果で監査レコードを選択します。</span><span class="sxs-lookup"><span data-stu-id="cb1ee-112">Select an audit record in the results.</span></span> <span data-ttu-id="cb1ee-113">**詳細**ポップアップで、[**詳細情報**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="cb1ee-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="cb1ee-114">アクティビティが電子メール転送に関連しているかどうかを判断するには、各監査レコードの詳細を参照する必要があります。</span><span class="sxs-lookup"><span data-stu-id="cb1ee-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="cb1ee-115">**ObjectId**: 変更されたメールボックスのエイリアス値。</span><span class="sxs-lookup"><span data-stu-id="cb1ee-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="cb1ee-116">**パラメーター**: _ForwardingSmtpAddress_は、ターゲットの電子メールアドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="cb1ee-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="cb1ee-117">**UserId**: **ObjectId**フィールドのメールボックスで電子メール転送を構成したユーザー。</span><span class="sxs-lookup"><span data-stu-id="cb1ee-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="cb1ee-118">詳細については、「[メールボックスのメール転送をセットアップするユーザーの特定](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cb1ee-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
