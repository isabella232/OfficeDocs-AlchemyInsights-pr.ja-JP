---
title: すべてのユーザーにグローバルな会社の署名または免責事項を追加します
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: ab0d3fc80b41b9017a6917817270438644f770b8
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243800"
---
# <a name="add-a-global-company-signature-or-disclaimer-for-all-users"></a><span data-ttu-id="05917-102">すべてのユーザーにグローバルな会社の署名または免責事項を追加します</span><span class="sxs-lookup"><span data-stu-id="05917-102">Add a global company signature or disclaimer for all users</span></span>

<span data-ttu-id="05917-103">ヒント: 組織全体の署名は、その内容に関係なく、免責事項とも呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="05917-103">Tip: An org-wide signature is also called a disclaimer, regardless of what it includes.</span></span>

1. <span data-ttu-id="05917-104">管理センターで、**[管理センター]** > **[Exchange]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="05917-104">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="05917-105">[メール フロー] の [ **ルール**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="05917-105">Under Mail flow, choose **Rules**.</span></span>
3. <span data-ttu-id="05917-106">[ **+**] (追加) アイコンをクリックし、[ **免責事項を適用する**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="05917-106">Click the **+** (Add) icon and choose **Apply disclaimers**.</span></span>
4. <span data-ttu-id="05917-107">ルールに名前を付けます。</span><span class="sxs-lookup"><span data-stu-id="05917-107">Give the rule a name.</span></span>
5. <span data-ttu-id="05917-108">[このルールを適用します] の **[すべてのメッセージに適用]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="05917-108">Under Apply this rule, choose **Apply to all messages**.</span></span>
6. <span data-ttu-id="05917-109">[実行する処理] の [ **免責事項を追加する**] はオンのままにします。</span><span class="sxs-lookup"><span data-stu-id="05917-109">Under Do the following, leave **Append the disclaimer** selected.</span></span>
7. <span data-ttu-id="05917-110">[ **テキストを入力**] をクリックして免責事項を入力します</span><span class="sxs-lookup"><span data-stu-id="05917-110">Click **Enter text** and type your disclaimer.</span></span>
8. <span data-ttu-id="05917-111">**[1 つ選択]** をクリックし、フォールバック オプションとして **[ラッピング]** を選択し、**[OK]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="05917-111">Click **Select one**, choose **Wrap** as a fallback option, and then click **OK**.</span></span> <span data-ttu-id="05917-112">これは、暗号化や別のメール設定のために免責事項を追加できない場合に、メッセージ エンベロープで免責事項がラップされることを意味します。</span><span class="sxs-lookup"><span data-stu-id="05917-112">This means that if the disclaimer can't be added because of encryption or another mail setting, it will be wrapped in a message envelope.</span></span>
9. <span data-ttu-id="05917-113">[**このルールを次の重大度レベルで監査する**] はオンのままにします。</span><span class="sxs-lookup"><span data-stu-id="05917-113">Leave **Audit this rule** with severity level selected.</span></span> <span data-ttu-id="05917-114">次に、メッセージ ログに使用する [低]、[中]、または [高] を選択します。</span><span class="sxs-lookup"><span data-stu-id="05917-114">Then choose Low, Medium, or High to be used in the message log.</span></span>
10. <span data-ttu-id="05917-115">先にテストしない場合は、[ **強制**] を選択して免責事項を即時に有効にします。</span><span class="sxs-lookup"><span data-stu-id="05917-115">Choose **Enforce** to turn on the disclaimer immediately, unless you want to test it first.</span></span>
11. <span data-ttu-id="05917-116">追加の条件や例外を含めるには、[ **その他のオプション**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="05917-116">Choose **More options** to include additional conditions or exceptions.</span></span>
12. <span data-ttu-id="05917-117">変更が終わったら [**保存**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="05917-117">When finished, click **Save**.</span></span>
13. <span data-ttu-id="05917-118">サポートが必要な場合</span><span class="sxs-lookup"><span data-stu-id="05917-118">Need more help?</span></span> [<span data-ttu-id="05917-119">免責事項の作成に関するビデオを見るか、記事全体を読んでください。</span><span class="sxs-lookup"><span data-stu-id="05917-119">Watch a video about creating disclaimers or read the full article.</span></span>](https://support.office.com/article/2d75860f-c527-4352-a7f6-73eba54c0c72?wt.mc_id=Chat_GlobalSignature)