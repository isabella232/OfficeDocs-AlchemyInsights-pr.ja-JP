---
title: TeamViewer を使用して Intune デバイスをリモート管理する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: e931b2092ab049bc01c600344cbd4702848abcd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798453"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="607d3-102">TeamViewer を使用して Intune デバイスをリモート管理する</span><span class="sxs-lookup"><span data-stu-id="607d3-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="607d3-103">Intune で管理されているデバイスは、[TeamViewer](https://www.teamviewer.com/) を使用してリモート管理できます。</span><span class="sxs-lookup"><span data-stu-id="607d3-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="607d3-104">TeamViewer を使用して Intune を管理するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="607d3-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="607d3-105">まず、TeamViewer から資格情報を取得して、Intune で TeamViewer Connector をセットアップします。</span><span class="sxs-lookup"><span data-stu-id="607d3-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="607d3-106">これにより、管理者は、[デバイス] の TeamViewer Connector UI で資格情報を入力できるようになります。これは、Intune と TeamViewer サービスのリンクを確立するための 1 回限りの操作です。</span><span class="sxs-lookup"><span data-stu-id="607d3-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="607d3-107">**パート 1: リモート デバイスとのセッションを開始する**</span><span class="sxs-lookup"><span data-stu-id="607d3-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="607d3-108">[**すべてのデバイス**] で、リモート セッションを開始するデバイスを選択します。</span><span class="sxs-lookup"><span data-stu-id="607d3-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="607d3-109">[**その他**] で、[**新しいリモート アシスタンス セッション**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="607d3-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="607d3-110">[**はい**] を選択して、リモート セッションを開始することを確認します。</span><span class="sxs-lookup"><span data-stu-id="607d3-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="607d3-111">"新しいリモート セッションの開始" 要求が TeamViewer サービスによって確認されると、デバイスの [概要] (または [必須項目]) ウィンドウの詳細覧に [**リモート アシスタンスを開始**] というオプションが表示されます。</span><span class="sxs-lookup"><span data-stu-id="607d3-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="607d3-112">[**さらに表示**] を選択してウィンドウを展開し、[リモート アシスタンス] の状態を表示します。</span><span class="sxs-lookup"><span data-stu-id="607d3-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="607d3-113">[**リモート セッションの開始**] を選択して管理者側でセッションを開始します。</span><span class="sxs-lookup"><span data-stu-id="607d3-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="607d3-114">TeamViewer バイナリ (Windows) をダウンロードすることを選択し、[**実行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="607d3-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="607d3-115">**注** TeamViewer Web サイトに開かれるいずれの Web ブラウザーのページも無視します。</span><span class="sxs-lookup"><span data-stu-id="607d3-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="607d3-116">TeamViewer アプリがデバイスに変更を加えることに関する要求に同意します (Windows のみ)。</span><span class="sxs-lookup"><span data-stu-id="607d3-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="607d3-117">TeamViewer アプリが起動し、リモート デバイスへの接続を認証するためのセッション コードが提供されます。</span><span class="sxs-lookup"><span data-stu-id="607d3-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="607d3-118">**パート 2: リモート セッションの対象デバイスでの操作**</span><span class="sxs-lookup"><span data-stu-id="607d3-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="607d3-119">Intune の企業ポータルを開きます。</span><span class="sxs-lookup"><span data-stu-id="607d3-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="607d3-120">"Your IT administrator is requesting control of this device for a remote assistance session (IT 管理者がリモート アシスタンス セッションのためにこのデバイスの制御を要求しています)" という通知フラグを見つけ、この通知を選択します。</span><span class="sxs-lookup"><span data-stu-id="607d3-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="607d3-121">TeamViewer アプリケーションをダウンロードすることを選択するか、App Store から TeamViewer アプリをダウンロードすることに同意し、[**実行**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="607d3-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="607d3-122">**注** TeamViewer Web サイトに開かれるいずれの Web ブラウザーのページも無視します。</span><span class="sxs-lookup"><span data-stu-id="607d3-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="607d3-123">TeamViewer アプリがデバイスに変更を加えることに関する要求に同意します (Windows のみ)。</span><span class="sxs-lookup"><span data-stu-id="607d3-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="607d3-124">TeamViewer アプリが起動し、リモート デバイスへの接続を認証するためのセッション コードが提供されます。</span><span class="sxs-lookup"><span data-stu-id="607d3-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="607d3-125">ポップアップ ウィンドウが表示され、セッションの開始を許可するかどうかの確認が求められます。</span><span class="sxs-lookup"><span data-stu-id="607d3-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="607d3-126">**注**: TeamViewer サービスによって生成されるセッション コードは、1 回限り使用できます。</span><span class="sxs-lookup"><span data-stu-id="607d3-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="607d3-127">接続が切れた場合は、次の操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="607d3-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="607d3-128">リモート デバイスおよび管理ワークステーション上で、TeamViewer アプリのインスタンスを閉じます。</span><span class="sxs-lookup"><span data-stu-id="607d3-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="607d3-129">リモート デバイスで企業ポータルを閉じます。</span><span class="sxs-lookup"><span data-stu-id="607d3-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="607d3-130">管理ポータルから [新しいリモート アシスタンス セッション] を開始します。</span><span class="sxs-lookup"><span data-stu-id="607d3-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="607d3-131">リモート デバイスで企業ポータルをもう一度開き、新しい通知を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="607d3-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="607d3-132">先ほどと同様、リモート デバイスと管理ワークステーションの両方で、TeamViewer アプリを開きます。</span><span class="sxs-lookup"><span data-stu-id="607d3-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>