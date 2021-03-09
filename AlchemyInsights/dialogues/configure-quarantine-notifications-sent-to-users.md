---
title: ユーザーに送信される検疫通知の構成
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 3e3e350f74b19420155c29cb282f065e7db6d4d7
ms.sourcegitcommit: 1f998ca586c90330fde515525432072f766d485b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527939"
---
# <a name="configure-quarantine-notifications-sent-to-users"></a><span data-ttu-id="cdb64-102">ユーザーに送信される検疫通知の構成</span><span class="sxs-lookup"><span data-stu-id="cdb64-102">Configure quarantine notifications sent to users</span></span>

<span data-ttu-id="cdb64-103">検疫の内容について、ユーザーに通知を送信します。</span><span class="sxs-lookup"><span data-stu-id="cdb64-103">To send notifications to your users about what's in quarantine:</span></span>

1. <span data-ttu-id="cdb64-104">管理センターで、**[管理センター]**、 > **[Exchange]**、 > **[保護]**、 > **[スパム フィルター]** の順で移動します。</span><span class="sxs-lookup"><span data-stu-id="cdb64-104">In the admin center, navigate to **admin centers** > **Exchange** > **Protection** > **spam filter**.</span></span>
2. <span data-ttu-id="cdb64-105">通知を有効にするスパム フィルター ポリシーを選択します。</span><span class="sxs-lookup"><span data-stu-id="cdb64-105">Select the spam filter policy for which you want to turn on notifications.</span></span>
3. <span data-ttu-id="cdb64-106">右側のウィンドウで、**[エンドユーザーのスパム通知の構成]** リンクを選択します。</span><span class="sxs-lookup"><span data-stu-id="cdb64-106">In the right pane, choose the **Configure End-user spam notifications** link.</span></span>
4. <span data-ttu-id="cdb64-107">次のダイアログボックスで、**[エンドユーザーへのスパム通知を有効にする]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="cdb64-107">In the next dialog box, choose **Enable end-user spam notifications**.</span></span> <span data-ttu-id="cdb64-108">[このポリシーのスパム通知を有効にする] を選択します。</span><span class="sxs-lookup"><span data-stu-id="cdb64-108">Choose to enable spam notifications for this policy.</span></span>
5. <span data-ttu-id="cdb64-109">**[エンド ユーザーのスパム通知を～日ごとに送信]** で、エンド ユーザーのスパム通知を送信する頻度を指定します。</span><span class="sxs-lookup"><span data-stu-id="cdb64-109">In **Send end-user spam notifications every (days)**, specify how often to send user spam notifications.</span></span> <span data-ttu-id="cdb64-110">既定値は 3 日です。</span><span class="sxs-lookup"><span data-stu-id="cdb64-110">The default is 3 days.</span></span> <span data-ttu-id="cdb64-111">1 ～ 15 日の間で指定できます。</span><span class="sxs-lookup"><span data-stu-id="cdb64-111">You can specify between 1 and 15 days.</span></span> <span data-ttu-id="cdb64-112">たとえば 7 日間を指定した場合の通知には、直前の 7 日間のユーザー宛のメッセージのうち、スパム検疫に転送されたすべてのメッセージのリストが含まれます。</span><span class="sxs-lookup"><span data-stu-id="cdb64-112">If you specify 7 days, for example, the notification will include a list of all messages intended for that user within the past 7 days that were sent to the spam quarantine instead.</span></span>
6. <span data-ttu-id="cdb64-113">**[通知の言語]** で、このポリシーにユーザーのスパム通知の作成に使用する言語を選択します。</span><span class="sxs-lookup"><span data-stu-id="cdb64-113">In **Notification language** choose the language in which to write user spam notifications for this policy.</span></span>
7. <span data-ttu-id="cdb64-114">[**保存**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="cdb64-114">Choose **Save**.</span></span>
