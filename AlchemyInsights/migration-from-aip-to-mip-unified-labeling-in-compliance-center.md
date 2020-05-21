---
title: コンプライアンス センターでの AIP から MIP/統合ラベル付けへの移行
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7ce9c387fc94f59674a922c5fe071fc0fb030344
ms.sourcegitcommit: e6d73d240669342fde9d4d25b0ee2838b7e43965
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/14/2020
ms.locfileid: "44282071"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="01425-102">コンプライアンス センターでの AIP から MIP/統合ラベル付けへの移行</span><span class="sxs-lookup"><span data-stu-id="01425-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="01425-103">セキュリティ/コンプライアンス センターで AIP ラベルから統合ラベル付けに移行するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="01425-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="01425-104">**Azure ポータルからの保護を有効にする**</span><span class="sxs-lookup"><span data-stu-id="01425-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="01425-105">まだ行っていない場合は、新しいブラウザー ウィンドウを開いて、[Azure ポータルにサインイン](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal)します。</span><span class="sxs-lookup"><span data-stu-id="01425-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="01425-106">**Azure Information Protection** ブレードに移動します。</span><span class="sxs-lookup"><span data-stu-id="01425-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="01425-107">たとえば、ハブ メニューで [**すべてのサービス**] をクリックし、[フィルタ] ボックスに「**情報**」と入力し始めます。</span><span class="sxs-lookup"><span data-stu-id="01425-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="01425-108">[**Azure Information Protection**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="01425-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="01425-109">これまでに Azure Information Protection ブレードにアクセスしたことがない場合は、このブレードをポータルに追加するための 1 回限りの[追加の手順](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="01425-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="01425-110">Azure Information Protection ブレードを開くには、[Azure Information Protection Premium プラン](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing)、または Rights Management を含む Office 365 プランが必要です。</span><span class="sxs-lookup"><span data-stu-id="01425-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="01425-111">これらのサブスクリプションのいずれかを持っているが、有効なサブスクリプションが見つからないというメッセージが表示される場合は、[Microsoft サポートに連絡](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support)するか、標準のサポート チャネルを使用してください。</span><span class="sxs-lookup"><span data-stu-id="01425-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="01425-112">[**管理**] メニュー オプションを見つけ、[**保護のアクティブ化**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="01425-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="01425-113">[**アクティブ化**] をクリックして、操作を確認します。</span><span class="sxs-lookup"><span data-stu-id="01425-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="01425-114">アクティブ化が完了すると、情報バーに「**アクティブ化は正常に終了しました**」と表示されます。</span><span class="sxs-lookup"><span data-stu-id="01425-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="01425-115">**Azure Information Protection ラベルを Office 365 セキュリティ/コンプライアンス センターに移行する**</span><span class="sxs-lookup"><span data-stu-id="01425-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="01425-116">グローバル管理者権限を持つユーザーとしてログインしていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="01425-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="01425-117">**Azure Information Protection** ブレードに移動します。</span><span class="sxs-lookup"><span data-stu-id="01425-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="01425-118">[**管理**] メニュー オプションから [**統合ラベル付け**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="01425-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="01425-119">[**Azure Information Protection - 統合ラベル付け**] ブレードで、[**アクティブ化**] をクリックし、オンラインの指示に従います。</span><span class="sxs-lookup"><span data-stu-id="01425-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="01425-120">**注**: セキュリティ/コンプライアンス センターの移行をアクティブ化する前に、適切な権限があることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="01425-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="01425-121">詳細については、次の記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="01425-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="01425-122">Azure Information Protection を構成するには、グローバル管理者である必要がありますか、それとも他の管理者に委任できますか?</span><span class="sxs-lookup"><span data-stu-id="01425-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="01425-123">セキュリティ/コンプライアンス センターへの移行後の管理者の役割に関する重要な情報。</span><span class="sxs-lookup"><span data-stu-id="01425-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="01425-124">セキュリティ/コンプライアンス センターへの AIP から統合ラベル付けの移行の詳細については、「[ラベルの移行](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="01425-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
