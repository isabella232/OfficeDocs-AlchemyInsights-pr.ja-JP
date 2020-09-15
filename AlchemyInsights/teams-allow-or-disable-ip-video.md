---
title: Teams で IP ビデオを許可または無効にする
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: cf2d67170f846db1d5d2f1ca8c8b50902e200e45
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670189"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="3dc20-102">Teams で IP ビデオを許可または無効にする</span><span class="sxs-lookup"><span data-stu-id="3dc20-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="3dc20-103">**会議ポリシーを変更または作成する**</span><span class="sxs-lookup"><span data-stu-id="3dc20-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="3dc20-104">会議ポリシーを変更または作成するには、**Microsoft Teams 管理センターにアクセスし、[会議]、[会議ポリシー]** の順に移動します。</span><span class="sxs-lookup"><span data-stu-id="3dc20-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="3dc20-105">一覧からポリシーを選択するか、**[追加]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="3dc20-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="3dc20-106">新しいポリシーを作成する場合は、名前と説明を追加します。</span><span class="sxs-lookup"><span data-stu-id="3dc20-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="3dc20-107">名前に特殊文字を含めたり、64 文字より長くしたりすることはできません。</span><span class="sxs-lookup"><span data-stu-id="3dc20-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="3dc20-108">設定を選び、**[保存]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="3dc20-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="3dc20-109">たとえば、多数のユーザーがいて、会議に必要な帯域幅を制限するとします。</span><span class="sxs-lookup"><span data-stu-id="3dc20-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="3dc20-110">「制限された帯域幅」という名前の新しいカスタム ポリシーを作成し、次の設定を無効にできます。</span><span class="sxs-lookup"><span data-stu-id="3dc20-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="3dc20-111">[**オーディオとビデオ**] で、</span><span class="sxs-lookup"><span data-stu-id="3dc20-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="3dc20-112">[クラウド記録を許可する] を無効にします。</span><span class="sxs-lookup"><span data-stu-id="3dc20-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="3dc20-113">[IP のビデオを許可する] を無効にします。</span><span class="sxs-lookup"><span data-stu-id="3dc20-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="3dc20-114">その後、ポリシーをユーザーに割り当てます。</span><span class="sxs-lookup"><span data-stu-id="3dc20-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="3dc20-115">**ユーザーに会議ポリシーを割り当てる**</span><span class="sxs-lookup"><span data-stu-id="3dc20-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="3dc20-116">Microsoft Teams 管理センターの左側のナビゲーションで、**[ユーザー]** に移動してユーザーをクリックします。</span><span class="sxs-lookup"><span data-stu-id="3dc20-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="3dc20-117">ユーザー名の左側をクリックしてユーザーを選択し、[**編集を設定する**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="3dc20-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="3dc20-118">[**会議ポリシー**] で割り当てるポリシーを選択し、[**適用**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="3dc20-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="3dc20-119">詳細については、「[Teams での会議ポリシーを管理する](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3dc20-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
