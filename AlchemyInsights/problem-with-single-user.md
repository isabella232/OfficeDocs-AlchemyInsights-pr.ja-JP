---
title: 単一ユーザーの問題
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430409"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="265ed-102">単一ユーザーの問題</span><span class="sxs-lookup"><span data-stu-id="265ed-102">Problem with single user</span></span>

- <span data-ttu-id="265ed-103">サービスがまだユーザーを評価する機会を与えていないため、ユーザーがプロビジョニングされていない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="265ed-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="265ed-104">プロビジョニングに必要な時間と、プロビジョニング構成ページの進行状況バーを確認します。</span><span class="sxs-lookup"><span data-stu-id="265ed-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="265ed-105">追加の詳細セクションで指定された一定の状態が、ユーザーが作成/更新/削除された日付より前の場合は、ユーザーがまだ評価されていないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="265ed-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="265ed-106">このシナリオでは、プロビジョニング サービスが終了するまで待つ必要があります。</span><span class="sxs-lookup"><span data-stu-id="265ed-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="265ed-107">サービスは、ソース システム (クラウド HR) 内のユーザーに対する変更のみを認識している点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="265ed-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="265ed-108">Azure AD が変更を検出して Active Directory に流し込むには、Azure AD のソース システムに有効な変更が必要です。</span><span class="sxs-lookup"><span data-stu-id="265ed-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="265ed-109">プロビジョニング サービスによってユーザーが評価され、プロビジョニングできないと判断されました。</span><span class="sxs-lookup"><span data-stu-id="265ed-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="265ed-110">属性ベースの範囲指定フィルターを設定した場合は、ユーザーが指定した条件を満たしていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="265ed-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="265ed-111">ユーザーがターゲット システムに既に存在し、ソースとターゲットのユーザーの状態が一致する場合、それ以上アクションは実行されません。</span><span class="sxs-lookup"><span data-stu-id="265ed-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="265ed-112">プロビジョニング サービスがユーザーのプロビジョニングを試みましたが、失敗しました。</span><span class="sxs-lookup"><span data-stu-id="265ed-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="265ed-113">これらのシナリオでは、プロビジョニング ログの「トラブルシューティングと推奨事項」タブを確認します。</span><span class="sxs-lookup"><span data-stu-id="265ed-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="265ed-114">オンプレミスの Active Directory または Azure AD に、ユーザーの必須属性がない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="265ed-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="265ed-115">たとえば、userPrincipalName または sAMAccountName 生成ルールが正しい値を生成していないとします。</span><span class="sxs-lookup"><span data-stu-id="265ed-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="265ed-116">一致する属性 (通常は employeeId) は、オンプレミスの Active Directory または Azure AD の一意のユーザーに対して解決されません。</span><span class="sxs-lookup"><span data-stu-id="265ed-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="265ed-117">たとえば、AD で同じ employeeId を持つユーザーが 2 人いて、サービスが同じソース エントリの重複対象エントリを示すエラー コードを返しているとします。</span><span class="sxs-lookup"><span data-stu-id="265ed-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="265ed-118">単一のユーザーとグループのログを確認するには、「[特定のユーザーグループに関する問題のプロビジョニング ログを確認する](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="265ed-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
