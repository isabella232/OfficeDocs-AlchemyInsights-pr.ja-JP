---
title: Intune 条件付きアクセスを監視
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/03/2021
ms.locfileid: "50428388"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="e8358-102">Intune 条件付きアクセスを監視</span><span class="sxs-lookup"><span data-stu-id="e8358-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="e8358-p101">条件付きアクセスで対象となるユーザーは、組織のアクセス要件を満たしていない場合には通知電子メールを受信します。この状態を解消するには、以下の 1 つ以上の解決策をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="e8358-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="e8358-105">デバイス登録が済んでいると想定される場合は、Intune ポータル サイト アプリを使い、デバイスがポータル サイトに表示されているかどうかを確認することを、ユーザーに勧めてください。</span><span class="sxs-lookup"><span data-stu-id="e8358-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="e8358-106">もし表示されていない場合、ユーザーがデバイスを登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e8358-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="e8358-107">Azure portal で **[Intune]** > **[デバイス ポリシー準拠]** の順に選びます。</span><span class="sxs-lookup"><span data-stu-id="e8358-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="e8358-108">デバイスのポリシー準拠レポートを表示して、ユーザーのデバイスがポリシー準拠と示されているかどうか確認するには、**モニター** で **[デバイスのポリシー準拠]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="e8358-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="e8358-109">Azure portal で **[Intune]** > **[デバイス ポリシー準拠]** の順に選びます。</span><span class="sxs-lookup"><span data-stu-id="e8358-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="e8358-110">**[管理]** で **[プロパティ]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="e8358-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="e8358-111">コンプライアンス ポリシーの一覧で、ユーザーのデバイスにプロファイルが割り当てられていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="e8358-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="e8358-112">プロファイルが割り当てられていない場合、Intune はデバイスの準拠状況を確認することができません。</span><span class="sxs-lookup"><span data-stu-id="e8358-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="e8358-113">ユーザーの条件付きアクセス割り当てを編集します。</span><span class="sxs-lookup"><span data-stu-id="e8358-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="e8358-114">Azure portal で、**Intune** > **条件付きアクセス** > **ポリシー** にアクセスし、一覧からポリシーを選択し、**ユーザーとグループ** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="e8358-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="e8358-115">特定のユーザーに対して特定のポリシーを対象とするには、それらのユーザーを **[対象リスト]** に追加します。</span><span class="sxs-lookup"><span data-stu-id="e8358-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="e8358-116">特定のユーザーに対して特定のポリシーを対象とするには、それらのユーザーを **[除外リスト]** に追加します。</span><span class="sxs-lookup"><span data-stu-id="e8358-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="e8358-117">**便利なリンク:**</span><span class="sxs-lookup"><span data-stu-id="e8358-117">**Helpful links:**</span></span>

- [<span data-ttu-id="e8358-118">デバイス コンプライアンスの概要</span><span class="sxs-lookup"><span data-stu-id="e8358-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="e8358-119">CA のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="e8358-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="e8358-120">トラブルシューティング ポリシー</span><span class="sxs-lookup"><span data-stu-id="e8358-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="e8358-121">Intune デバイス コンプライアンスの監視</span><span class="sxs-lookup"><span data-stu-id="e8358-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="e8358-122">これらの手順は、Azure Active Directory 機能の条件付きアクセスに関するトラブルシューティングを行う場合にのみ役立ちます。</span><span class="sxs-lookup"><span data-stu-id="e8358-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="e8358-123">また、Exchange ポリシーを使用してメール アクセスをブロックしているデバイスを検疫することも可能です。</span><span class="sxs-lookup"><span data-stu-id="e8358-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="e8358-124">Exchange デバイス管理の詳細については、[**こちら**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e8358-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
