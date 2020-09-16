---
title: VPN に関連する問題
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
- "1545"
- "9000076"
ms.openlocfilehash: 3c031725c92f5d7af7c0dd0c37ea34fecf4792c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47726096"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="04c98-102">VPN に関連する問題</span><span class="sxs-lookup"><span data-stu-id="04c98-102">VPN related issues</span></span>

<span data-ttu-id="04c98-103">MDM クライアントの VPN 接続を正常に実装するには、VPN インフラストラクチャの要件を正しく反映する展開済みのプロファイルが存在している必要があります。</span><span class="sxs-lookup"><span data-stu-id="04c98-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="04c98-104">調査しているクライアント プラットフォームの適切な設定については、次を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04c98-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="04c98-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune (Windows 10 および Windows Holographic デバイスを設定して Intune を使用した VPN 接続を追加する)</span><span class="sxs-lookup"><span data-stu-id="04c98-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="04c98-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune (Microsoft Intune で iOS デバイスおよび iPadOS デバイスに VPN 設定を追加する)</span><span class="sxs-lookup"><span data-stu-id="04c98-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="04c98-107">Android device settings to configure VPN in Intune (Intune で VPN を構成するための Android デバイスの設定)</span><span class="sxs-lookup"><span data-stu-id="04c98-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="04c98-108">Add VPN settings on macOS devices in Microsoft Intune (Microsoft Intune で macOS デバイスおよび iPadOS デバイスに VPN 設定を追加する)</span><span class="sxs-lookup"><span data-stu-id="04c98-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="04c98-109">VPN プロファイルで認証に基づく証明書が使用されている場合、VPN プロファイルにリンクされているルート証明書プロファイルとクライアント認証証明書プロファイルが正常に展開されていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="04c98-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="04c98-110">**一般的な問題**</span><span class="sxs-lookup"><span data-stu-id="04c98-110">**Common Issues**</span></span>

<span data-ttu-id="04c98-111">**VPN プロファイルをデバイスに展開しました。正常に展開されたと Intune に表示されていますが、デバイスが VPN に接続されていません。**</span><span class="sxs-lookup"><span data-stu-id="04c98-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="04c98-112">正常な状態とは、Intune が構成通りにプロファイルを展開したという意味です。</span><span class="sxs-lookup"><span data-stu-id="04c98-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="04c98-113">ただし、これらの構成がお使いのネットワークや認証要件に適合していない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="04c98-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="04c98-114">接続の試行の詳細については、(VPN サーバーと NPS/Radius サーバー上の) インフラストラクチャと認証サービスのログを確認します。</span><span class="sxs-lookup"><span data-stu-id="04c98-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="04c98-115">ログを収集して確認するには、ネットワーク インフラストラクチャ チームまたはサードパーティ VPN ベンダーと連携する必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="04c98-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="04c98-116">**iOS 用のカスタム VPN を構成した際に、アプリ単位の VPN 機能が利用できません。**</span><span class="sxs-lookup"><span data-stu-id="04c98-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="04c98-117">Intune での iOS デバイス用のアプリ単位の VPN は現在、特定の一覧に含まれるプロバイダーとパートナーに対して提供されており、これらのプロバイダーとパートナーはまた、証明書の前提条件を満たしてからでないとアプリ単位の VPN を構成できません。</span><span class="sxs-lookup"><span data-stu-id="04c98-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="04c98-118">詳細については、「[Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune (Intune で iOS/iPadOS 用のアプリ単位の仮想プライベート ネットワーク (NPN) をセットアップする)](https://docs.microsoft.com/intune/vpn-setting-configure-per-app)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04c98-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="04c98-119">Intune の VPN のすべての接続タイプの詳細については、「[ (VPN サーバーに接続するための VPN プロファイルを Intune で作成する)](https://docs.microsoft.com/intune/vpn-settings-configure)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04c98-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="04c98-120">**構成済みのドメインにアクセスしたときに iOS のオンデマンド VPN がトリガーされない**</span><span class="sxs-lookup"><span data-stu-id="04c98-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="04c98-121">自動 VPN 設定をテストするには、次の値を設定します。</span><span class="sxs-lookup"><span data-stu-id="04c98-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="04c98-122">I want to do the following (次の操作を実行する): **Evaluate each connection attempt (それぞれの接続の試行を評価する)**</span><span class="sxs-lookup"><span data-stu-id="04c98-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="04c98-123">Choose whether to connect (接続するかどうかの選択): **Connect if needed (必要な場合は接続する)**</span><span class="sxs-lookup"><span data-stu-id="04c98-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="04c98-124">When users access these domains (ユーザーがこれらのドメインにアクセスした場合): **target (ターゲット)** *domain name (ドメイン名)*</span><span class="sxs-lookup"><span data-stu-id="04c98-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="04c98-125">上記の構成が正常に動作しない場合は、次の要素を追加します。</span><span class="sxs-lookup"><span data-stu-id="04c98-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="04c98-126">When this URL is unreachable, force connect the VPN (この URL に接続できない場合は、VPN を強制接続する): **BADURL**</span><span class="sxs-lookup"><span data-stu-id="04c98-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>