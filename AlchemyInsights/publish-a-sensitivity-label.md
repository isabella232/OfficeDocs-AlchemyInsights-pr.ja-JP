---
title: 秘密度ラベル用に暗号化を構成する方法
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11015"
- "9000181"
ms.openlocfilehash: 2f09de066bf234bcc92935f662f2d3b1077d0217
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233791"
---
# <a name="how-to-publish-a-sensitivity-label"></a><span data-ttu-id="3071d-102">秘密度ラベル用に暗号化を構成する方法</span><span class="sxs-lookup"><span data-stu-id="3071d-102">How to publish a sensitivity label</span></span>

1. <span data-ttu-id="3071d-103">[Office 365 セキュリティ/コンプライアンス センター]、[**分類**] > 、[**秘密度レベル**] の順に移動します。</span><span class="sxs-lookup"><span data-stu-id="3071d-103">Go to the Office 365 Security & Compliance Center > **Classification** > **Sensitivity labels**.</span></span>

1. <span data-ttu-id="3071d-104">[秘密度ラベル] ページで、[**ラベル ポリシー**] タブを選択し、[**ラベルの公開**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3071d-104">On the Sensitivity labels page, select the **Label policies** tab, and then select **Publish labels**.</span></span>

1. <span data-ttu-id="3071d-105">[**発行する秘密度ラベルの選択**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="3071d-105">Select **Choose sensitivity labels to publish**.</span></span> <span data-ttu-id="3071d-106">アプリとサービスで使用するラベルを選択し、[**追加**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3071d-106">Select the labels that you want to make available in apps and to services, and then select **Add**.</span></span>

    <span data-ttu-id="3071d-107">**重要**: サブラベルを選択する場合は、必ず親ラベルも選択してください。</span><span class="sxs-lookup"><span data-stu-id="3071d-107">**Important**: If you select a sublabel, make sure you also select its parent label.</span></span>

1. <span data-ttu-id="3071d-108">選択したラベルを確認します。</span><span class="sxs-lookup"><span data-stu-id="3071d-108">Review the selected labels.</span></span> <span data-ttu-id="3071d-109">変更を加えるには、[**編集**] を選択します。 それ以外の場合は、[**次へ**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3071d-109">To make any changes, select **Edit**; otherwise, select **Next**.</span></span>

1. <span data-ttu-id="3071d-110">指示に従ってポリシー設定を構成します。</span><span class="sxs-lookup"><span data-stu-id="3071d-110">Follow the prompts to configure the policy settings.</span></span>

1. <span data-ttu-id="3071d-111">異なるユーザーや場所に対して、異なるポリシー設定が必要な場合は、次の手順を繰り返します。</span><span class="sxs-lookup"><span data-stu-id="3071d-111">Repeat these steps if you need different policy settings for different users or locations.</span></span> <span data-ttu-id="3071d-112">たとえば、ユーザーのグループにラベルを追加したり、ユーザーのサブセットに別の既定のラベルを作成したりできます。</span><span class="sxs-lookup"><span data-stu-id="3071d-112">For example, you want additional labels for a group of users, or a different default label for a subset of users.</span></span>

1. <span data-ttu-id="3071d-113">複数のラベル ポリシーを作成すると、ユーザーまたは場所の競合が発生することがあります。ポリシーの順序を確認し、必要に応じてこれらを上下に移動します。</span><span class="sxs-lookup"><span data-stu-id="3071d-113">If you create more than one label policy that might result in a conflict for a user or location, review the policy order and if necessary, move them up or down.</span></span> <span data-ttu-id="3071d-114">ラベル ポリシーの順序を変更するには、[**その他のアクション**] の [**...**] を選択して、[**上へ移動**] または [**下へ移動**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="3071d-114">To change the order of a label policy, select **...** for **More actions**, and then select **Move up** or **Move down**.</span></span>

<span data-ttu-id="3071d-115">ウィザードを完了すると、ラベル ポリシーが自動的に発行されます。</span><span class="sxs-lookup"><span data-stu-id="3071d-115">Completing the wizard automatically publishes the label policy.</span></span>