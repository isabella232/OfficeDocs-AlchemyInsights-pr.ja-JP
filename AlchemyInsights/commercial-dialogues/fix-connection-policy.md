---
title: 接続 ポリシーを修正
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
- "9000760"
- "7391"
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751417"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="05342-102">接続 ポリシーを修正</span><span class="sxs-lookup"><span data-stu-id="05342-102">Fix connection policy</span></span>

<span data-ttu-id="05342-103">送信 IP アドレスは、接続フィルター ポリシーで安全とマークされたため、メールは安全とマークされ、ユーザーの受信トレイに配信されました。</span><span class="sxs-lookup"><span data-stu-id="05342-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="05342-104">ポリシーを確認するには、次の操作を行います。</span><span class="sxs-lookup"><span data-stu-id="05342-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="05342-105">[ Office 365 セキュリティ/コンプライアンス センター](https://go.microsoft.com/fwlink/p/?linkid=2077143)に移動し、**[脅威の管理]** > **[ポリシー]** > [[スパム対策]](https://go.microsoft.com/fwlink/?linkid=2101518)に移動します。</span><span class="sxs-lookup"><span data-stu-id="05342-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="05342-106">**[カスタム]** タブで、 **[接続フィルターポリシー]** 選択し、 **[ポリシーの編集]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="05342-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="05342-107">**[IP 許可]** リストを確認します。</span><span class="sxs-lookup"><span data-stu-id="05342-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="05342-108">**[セーフ リスト]** が有効になっていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="05342-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="05342-109">Microsoft は、信頼できる送信者のサード パーティ ソースにサブスクライブしています。</span><span class="sxs-lookup"><span data-stu-id="05342-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="05342-110">**[セーフ リスト]** 有効になっている場合、信頼できる送信者に誤ってスパムのマークをつけないようにします。</span><span class="sxs-lookup"><span data-stu-id="05342-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="05342-111">このオプションを選択すると、誤検知 (スパムとして分類される正常なメール) の受信数が減少するため、選択することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="05342-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
