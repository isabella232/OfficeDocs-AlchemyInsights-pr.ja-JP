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
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366433"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="97651-102">Exchange の条件付きアクセスを監視する</span><span class="sxs-lookup"><span data-stu-id="97651-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="97651-p101">条件付きアクセスで対象となるユーザーは、組織のアクセス要件を満たしていない場合には通知電子メールを受信します。この状態を解消するには、以下の 1 つ以上の解決策をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="97651-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="97651-p102">そのデバイスが登録されていると推測される場合、ポータル サイト アプリに移動して、ポータル サイトに表示されていることを確認するようユーザーに勧めます。表示されない場合、ユーザーはそのデバイスを登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="97651-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="97651-p103">Azure portal で、[Intune > デバイスコンプライアンス] に移動します。[モニター] の [デバイスのコンプライアンス] をクリックします。デバイスコンプライアンスレポートを表示して、ユーザーのデバイスが準拠しているとしてマークされていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="97651-p103">In the Azure portal go to Intune > Device compliance. Under Monitor click Device compliance. View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="97651-p104">Azure portal で、[Intune > デバイスコンプライアンス] に移動します。[管理] で、[ポリシー] をクリックします。コンプライアンスポリシーの一覧で、プロファイルがユーザーのデバイスに割り当てられていることを確認します。プロファイルが割り当てられていない場合、Intune はデバイスのコンプライアンスの状態を確認できません。</span><span class="sxs-lookup"><span data-stu-id="97651-p104">In the Azure portal go to Intune > Device compliance. Under Manage, click Policies. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="97651-114">ユーザーの条件付きアクセス割り当てを編集します。</span><span class="sxs-lookup"><span data-stu-id="97651-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="97651-115">Azure portal で、[ **Intune**  >  **条件付きアクセス**  >  **ポリシー**] に移動します。</span><span class="sxs-lookup"><span data-stu-id="97651-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="97651-116">リストからポリシーを選択します。</span><span class="sxs-lookup"><span data-stu-id="97651-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="97651-117">[ユーザーとグループ] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="97651-117">Click Users and groups.</span></span>
4. <span data-ttu-id="97651-p105">特定のユーザーに対して特定のポリシーを対象とするには、[必要] リストに追加します。対象ポリシーから特定のユーザーを除外するには、[必要なし] リストに追加します。</span><span class="sxs-lookup"><span data-stu-id="97651-p105">To target a certain policy at someone, add them to the Include list. To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="97651-120">便利なリンク:</span><span class="sxs-lookup"><span data-stu-id="97651-120">Helpful links:</span></span>

[<span data-ttu-id="97651-121">デバイス コンプライアンスの概要</span><span class="sxs-lookup"><span data-stu-id="97651-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="97651-122">CA のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="97651-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="97651-123">トラブルシューティング ポリシー</span><span class="sxs-lookup"><span data-stu-id="97651-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="97651-124">Intune デバイスコンプライアンスの監視</span><span class="sxs-lookup"><span data-stu-id="97651-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="97651-125">注: これらの手順は、Azure Active Directory 機能の条件付きアクセスのトラブルシューティングにのみ役立ちます。</span><span class="sxs-lookup"><span data-stu-id="97651-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="97651-126">Exchange ポリシーを使用して、電子メールへのアクセスをブロックするデバイスを検疫することもできます。</span><span class="sxs-lookup"><span data-stu-id="97651-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="97651-127">Exchange デバイス管理の詳細については、 [こちら](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="97651-127">More information on Exchange device management can be found [here](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span></span>
