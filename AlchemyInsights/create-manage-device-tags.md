---
title: デバイス タグまたはグループの作成と管理
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2021
ms.locfileid: "52732088"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="10f07-102">デバイス タグまたはグループの作成と管理</span><span class="sxs-lookup"><span data-stu-id="10f07-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="10f07-103">デバイスにタグを追加して、論理グループ アフィリエーションを作成します。</span><span class="sxs-lookup"><span data-stu-id="10f07-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="10f07-104">デバイス タグはネットワークの適切なマッピングをサポートし、さまざまなタグを添付してコンテキストをキャプチャし、インシデントの一部として動的リストを作成できるようにします。</span><span class="sxs-lookup"><span data-stu-id="10f07-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="10f07-105">タグは、デバイス リスト ビューでフィルターとして使用したり、デバイスをグループ化するために使用できます。</span><span class="sxs-lookup"><span data-stu-id="10f07-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="10f07-106">デバイスのグループ化の詳細については、「[デバイス タグの作成と管理](/microsoft-365/security/defender-endpoint/machine-tags)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="10f07-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="10f07-107">次の方法でデバイスにタグを追加できます。</span><span class="sxs-lookup"><span data-stu-id="10f07-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="10f07-108">ポータルを使用する</span><span class="sxs-lookup"><span data-stu-id="10f07-108">Using the portal</span></span>

- <span data-ttu-id="10f07-109">レジストリ キー値を設定する</span><span class="sxs-lookup"><span data-stu-id="10f07-109">Setting a registry key value</span></span>
 
<span data-ttu-id="10f07-110">**注:** タグがデバイスに追加されてから、デバイス リストおよびデバイス ページにタグが表示されるまでには、遅延が発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="10f07-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="10f07-111">API を使用してデバイス タグを追加するには、「[デバイス タグ API の追加または削除](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="10f07-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="10f07-112">ポータルを使用してデバイス タグを追加および管理する</span><span class="sxs-lookup"><span data-stu-id="10f07-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="10f07-113">タグを管理するデバイスを選択します。</span><span class="sxs-lookup"><span data-stu-id="10f07-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="10f07-114">次のいずれかのビューからデバイスを選択または検索できます。</span><span class="sxs-lookup"><span data-stu-id="10f07-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="10f07-115">**セキュリティ運用ダッシュボード** [アクティブなアラートがある上位デバイス] セクションからデバイス名を選択します。</span><span class="sxs-lookup"><span data-stu-id="10f07-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="10f07-116">**アラート キュー** - アラート キューからデバイス アイコンの横にあるデバイス名を選択します。</span><span class="sxs-lookup"><span data-stu-id="10f07-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="10f07-117">**デバイス リスト** - デバイスのリストからデバイス名を選択します。</span><span class="sxs-lookup"><span data-stu-id="10f07-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="10f07-118">**検索ボックス** - ドロップダウン メニューから [デバイス] を選択し、デバイス名を入力します。</span><span class="sxs-lookup"><span data-stu-id="10f07-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="10f07-119">ファイル ビューと IP ビューからアラート ページにアクセスすることもできます。</span><span class="sxs-lookup"><span data-stu-id="10f07-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="10f07-120">[応答] アクションの行から **[タグの管理]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="10f07-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="10f07-121">入力してタグを検索または作成します。</span><span class="sxs-lookup"><span data-stu-id="10f07-121">Type to find or create tags.</span></span>

<span data-ttu-id="10f07-122">タグがデバイス ビューに追加され、デバイス リスト ビューに反映されます。</span><span class="sxs-lookup"><span data-stu-id="10f07-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="10f07-123">その後、[タグ] フィルターを使用して、関連するデバイスのリストを表示できます。</span><span class="sxs-lookup"><span data-stu-id="10f07-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="10f07-124">詳細については、「[デバイス タグの作成と管理](/microsoft-365/security/defender-endpoint/machine-tags)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="10f07-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>