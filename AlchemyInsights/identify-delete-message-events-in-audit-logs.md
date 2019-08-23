---
title: 監査ログの削除メッセージイベントを識別する
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: b358b7944b82182a8551d64701e6879a01816524
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539214"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="9d7ae-102">削除された電子メールメッセージの監査ログ</span><span class="sxs-lookup"><span data-stu-id="9d7ae-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="9d7ae-103">2019年1月以降、Microsoft は既定でメールボックス監査ログをオンにしています。</span><span class="sxs-lookup"><span data-stu-id="9d7ae-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="9d7ae-104">または、特定のユーザーのメッセージイベントの削除を確認するには、監査の削除アクションを手動で有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d7ae-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="9d7ae-105">メールボックス監査ログが組織または特定のユーザーに対して既に有効になっている場合は、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="9d7ae-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="9d7ae-106">[Office 365 セキュリティ & コンプライアンスセンター](https://protection.office.com/)にログインする</span><span class="sxs-lookup"><span data-stu-id="9d7ae-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="9d7ae-107">[**検索と調査**] をクリックして、[**監査ログの検索**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="9d7ae-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="9d7ae-108">[**開始日**] フィールドと [**終了日**] フィールドで日付範囲を選択します。</span><span class="sxs-lookup"><span data-stu-id="9d7ae-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="9d7ae-109">調査するユーザーのユーザー名 (アイテムを削除したユーザー) を指定します。</span><span class="sxs-lookup"><span data-stu-id="9d7ae-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="9d7ae-110">[**アクティビティ**] フィールドで、[削除済み**アイテムフォルダーからメッセージ**を削除し、削除済み**アイテムフォルダーにメッセージを移動**しました] を選択します。</span><span class="sxs-lookup"><span data-stu-id="9d7ae-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="9d7ae-111">**[検索]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="9d7ae-111">Click **Search**.</span></span>

<span data-ttu-id="9d7ae-112">結果から、監査レコードを選択します。</span><span class="sxs-lookup"><span data-stu-id="9d7ae-112">In the results, select an audit record.</span></span> <span data-ttu-id="9d7ae-113">詳細ポップアップで、[**詳細情報**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="9d7ae-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="9d7ae-114">削除されたアイテムに関する追加情報 (たとえば、アイテムが削除されたときの件名やアイテムの場所) は、 **AffectedItems**フィールドに表示されます。</span><span class="sxs-lookup"><span data-stu-id="9d7ae-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="9d7ae-115">**Clientinfostring**プロパティは、outlook、web 上の outlook (旧称 Outlook web App)、またはその他のデバイスで削除が行われた場合に表示されます。</span><span class="sxs-lookup"><span data-stu-id="9d7ae-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="9d7ae-116">詳細については、「[メールボックスのメール転送をセットアップするユーザーの特定](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9d7ae-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="9d7ae-117">**注**: 監査ログ機能を使用して、削除されたアイテムを取得することはできません。</span><span class="sxs-lookup"><span data-stu-id="9d7ae-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="9d7ae-118">削除済みメッセージを Outlook on the web で取得するには、「 [Outlook Web App で削除済みアイテムを回復](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9d7ae-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
