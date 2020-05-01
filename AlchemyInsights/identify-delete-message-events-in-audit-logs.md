---
title: 監査ログのメッセージ イベントの削除を特定する
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 797a4b1146862faf91d2b9e8d74feade90f71650
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716501"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="5eafe-102">削除されたメール メッセージの監査ログ</span><span class="sxs-lookup"><span data-stu-id="5eafe-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="5eafe-103">2019 年 1 月から、Microsoft では、標準でメールボックス監査が有効になっています。</span><span class="sxs-lookup"><span data-stu-id="5eafe-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="5eafe-104">それ以外の場合、特定のユーザーのメッセージの削除を確認するためには、監査の削除操作を手動で有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="5eafe-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="5eafe-105">組織または特定のユーザーのメールボックス監査ログが既に有効になっている場合は、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="5eafe-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="5eafe-106">[Microsoft 365 セキュリティ/コンプライアンス センター](https://protection.office.com/)にログインします</span><span class="sxs-lookup"><span data-stu-id="5eafe-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="5eafe-107">[**検索と調査**] と [**監査ログ検索**]をクリックする。</span><span class="sxs-lookup"><span data-stu-id="5eafe-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="5eafe-108">[**開始日付**] と [**終了日付**] フィールドで日付範囲を選択します。</span><span class="sxs-lookup"><span data-stu-id="5eafe-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="5eafe-109">調べたいユーザー(アイテムを削除したユーザー) のユーザー名を指定します。</span><span class="sxs-lookup"><span data-stu-id="5eafe-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="5eafe-110">[**アクティビティ**]フィールドで、[**削除済みアイテム フォルダーからの削除済みメッセージ**] と [**削除済みアイテム フォルダーに移動済みのメッセージ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="5eafe-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="5eafe-111">[**検索**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="5eafe-111">Click **Search**.</span></span>

<span data-ttu-id="5eafe-112">結果から、[監査レコード] を選択します。</span><span class="sxs-lookup"><span data-stu-id="5eafe-112">In the results, select an audit record.</span></span> <span data-ttu-id="5eafe-113">詳細ポップアップから、 [**詳細情報**]をクリックします。</span><span class="sxs-lookup"><span data-stu-id="5eafe-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="5eafe-114">削除された項目に関する追加情報(件名、項目が削除されたときの場所など) は、 [**対象アイテム**] フィールドに表示されます。</span><span class="sxs-lookup"><span data-stu-id="5eafe-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="5eafe-115">**ClientInfoString** プロパティが、Outlook、Outlook on the web (旧称 Outlook Web App)、またはその他のデバイス上で削除が発生したかどうかを表示します。</span><span class="sxs-lookup"><span data-stu-id="5eafe-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="5eafe-116">詳細については、 [メールボックスへの転送を誰が設定したのか判別する](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5eafe-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="5eafe-117">**注意**: 監査ログ機能を使用して、削除したアイテムを復元することはできません。</span><span class="sxs-lookup"><span data-stu-id="5eafe-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="5eafe-118">Outlook on the web で削除済みのメッセージを取得するには、[Outlook Web App で 削除済みアイテムを復元する](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5eafe-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
