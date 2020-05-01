---
title: 監査ログ内のメールボックスで外部のメール転送を特定する
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716465"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="702f5-102">外部のメール転送がメールボックスで構成された際に、それを特定する</span><span class="sxs-lookup"><span data-stu-id="702f5-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="702f5-103">Microsoft 365 ユーザーが外部のメール転送をメールボックスで構成すると、このアクティビティは **Set-Mailbox** コマンドレットの一部として監査されます。</span><span class="sxs-lookup"><span data-stu-id="702f5-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="702f5-104">セキュリティ/コンプライアンス センターで監査ログ検索を使用すると、アクティビティを表示できます。</span><span class="sxs-lookup"><span data-stu-id="702f5-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="702f5-105">[Microsoft 365 セキュリティ/コンプライアンス センター](https://protection.office.com/)にログインします。</span><span class="sxs-lookup"><span data-stu-id="702f5-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="702f5-106">**[検索]** > **[監査ログの検索]** ページに移動します。</span><span class="sxs-lookup"><span data-stu-id="702f5-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="702f5-107">[**開始日**] と [**終了日**] フィールドで日付範囲を選択します。</span><span class="sxs-lookup"><span data-stu-id="702f5-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="702f5-108">ユーザー名を指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="702f5-108">You don't need to specify a username.</span></span> <span data-ttu-id="702f5-109">[**アクティビティ**] フィールドが [**すべてのアクティビティの結果を表示**] と設定されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="702f5-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="702f5-110">[**検索**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="702f5-110">Click **Search**.</span></span>

<span data-ttu-id="702f5-111">結果で、[**結果をフィルター**] をクリックし、[アクティビティ] フィルター ボックスに「**Set-Mailbox**」と入力します。</span><span class="sxs-lookup"><span data-stu-id="702f5-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="702f5-112">結果で、監査レコードを選択します。</span><span class="sxs-lookup"><span data-stu-id="702f5-112">Select an audit record in the results.</span></span> <span data-ttu-id="702f5-113">[**詳細**] ポップアップから、[**詳細情報**]をクリックします。</span><span class="sxs-lookup"><span data-stu-id="702f5-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="702f5-114">アクティビティがメールの転送に関連しているかどうかを判断するには、各監査レコードの詳細を確認する必要があります。</span><span class="sxs-lookup"><span data-stu-id="702f5-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="702f5-115">**ObjectId**: 変更されたメールボックスのエイリアス値。</span><span class="sxs-lookup"><span data-stu-id="702f5-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="702f5-116">**パラメーター**: _ForwardingSmtpAddress_は、送信先のメール アドレスを示します。</span><span class="sxs-lookup"><span data-stu-id="702f5-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="702f5-117">**UserId**: [**ObjectId**] フィールドのメールボックスでメール転送を構成したユーザー。</span><span class="sxs-lookup"><span data-stu-id="702f5-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="702f5-118">詳細については、「[メールボックスの電子メール転送を誰が設定したかを判別する](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="702f5-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
