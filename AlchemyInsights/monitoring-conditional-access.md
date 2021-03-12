---
title: 条件付きアクセスを監視する
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708679"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="1c0cf-102">Exchange の条件付きアクセスを監視する</span><span class="sxs-lookup"><span data-stu-id="1c0cf-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="1c0cf-p101">条件付きアクセスで対象となるユーザーは、組織のアクセス要件を満たしていない場合には通知電子メールを受信します。この状態を解消するには、以下の 1 つ以上の解決策をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="1c0cf-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="1c0cf-p102">そのデバイスが登録されていると推測される場合、ポータル サイト アプリに移動して、ポータル サイトに表示されていることを確認するようユーザーに勧めます。表示されない場合、ユーザーはそのデバイスを登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1c0cf-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="1c0cf-107">Azure portal で [Intune]、[デバイス ポリシー準拠] の順に選びます。</span><span class="sxs-lookup"><span data-stu-id="1c0cf-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="1c0cf-108">[監視] の下の、[デバイス準拠] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="1c0cf-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="1c0cf-109">デバイス準拠レポートで、ユーザーのデバイスが準拠としてマークされていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="1c0cf-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="1c0cf-110">Azure portal で [Intune]、[デバイス ポリシー準拠] の順に選びます。</span><span class="sxs-lookup"><span data-stu-id="1c0cf-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="1c0cf-111">[管理] で [プロパティ] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="1c0cf-111">Under Manage, click Policies.</span></span> <span data-ttu-id="1c0cf-112">コンプライアンス ポリシーの一覧で、ユーザーのデバイスにプロファイルが割り当てられていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="1c0cf-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="1c0cf-113">プロファイルが割り当てられていない場合、Intune はデバイスの準拠状況を確認することができません。</span><span class="sxs-lookup"><span data-stu-id="1c0cf-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="1c0cf-114">ユーザーの条件付きアクセス割り当てを編集します。</span><span class="sxs-lookup"><span data-stu-id="1c0cf-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="1c0cf-115">Azure ポータルで、**[Intune]**  >  **[条件付きアクセス]**  >  **[ポリシー]** と移動します。</span><span class="sxs-lookup"><span data-stu-id="1c0cf-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="1c0cf-116">一覧からポリシーを選択します。</span><span class="sxs-lookup"><span data-stu-id="1c0cf-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="1c0cf-117">[ユーザーとグループ] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="1c0cf-117">Click Users and groups.</span></span>
4. <span data-ttu-id="1c0cf-118">特定のユーザーに対して特定のポリシーを対象とするには、それらのユーザーを [対象リスト] に追加します。</span><span class="sxs-lookup"><span data-stu-id="1c0cf-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="1c0cf-119">特定のユーザーに対して特定のポリシーを対象外とするには、それらのユーザーを [除外リスト] に追加します。</span><span class="sxs-lookup"><span data-stu-id="1c0cf-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="1c0cf-120">便利なリンク:</span><span class="sxs-lookup"><span data-stu-id="1c0cf-120">Helpful links:</span></span>

[<span data-ttu-id="1c0cf-121">デバイス コンプライアンスの概要</span><span class="sxs-lookup"><span data-stu-id="1c0cf-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="1c0cf-122">CA のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="1c0cf-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="1c0cf-123">トラブルシューティング ポリシー</span><span class="sxs-lookup"><span data-stu-id="1c0cf-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="1c0cf-124">Intune デバイス コンプライアンスの監視</span><span class="sxs-lookup"><span data-stu-id="1c0cf-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="1c0cf-125">注: これらの手順は、Azure Active Directory 機能の条件付きアクセスに関するトラブルシューティングを行う場合にのみ役立ちます。</span><span class="sxs-lookup"><span data-stu-id="1c0cf-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="1c0cf-126">また、Exchange ポリシーを使用してメール アクセスをブロックしているデバイスを検疫することも可能です。</span><span class="sxs-lookup"><span data-stu-id="1c0cf-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="1c0cf-127">Exchange デバイス管理の詳細については、[こちら](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1c0cf-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
