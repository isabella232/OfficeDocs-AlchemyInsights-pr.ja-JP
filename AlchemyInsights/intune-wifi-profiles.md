---
title: Intune Wi-Fi プロファイル
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/29/2020
ms.locfileid: "46556228"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="a6aac-102">Intune Wi-Fi プロファイル</span><span class="sxs-lookup"><span data-stu-id="a6aac-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="a6aac-103">MDM クライアントの Wi-Fi 接続を正常に実装するには、Wi-Fi インフラストラクチャの要件を反映する正しく展開されたプロファイルが存在している必要があります。</span><span class="sxs-lookup"><span data-stu-id="a6aac-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="a6aac-104">調査しているクライアント プラットフォームの適切な設定を確認するには、次を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6aac-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="a6aac-105">Add Wi-Fi settings for devices running Android in Microsoft Intune (Android を実行するデバイス用に Microsoft Intune で Wi-Fi 設定を追加する)</span><span class="sxs-lookup"><span data-stu-id="a6aac-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="a6aac-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune (Microsoft Intune で、Android Enterprise 専用の完全に管理されたデバイスに Wi-Fi 設定を追加する)</span><span class="sxs-lookup"><span data-stu-id="a6aac-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="a6aac-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune (Microsoft Intune で iOS デバイスおよび iPadOS デバイス用の Wi-Fi 設定を追加する)</span><span class="sxs-lookup"><span data-stu-id="a6aac-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="a6aac-108">Add Wi-Fi settings for Windows 10 and later devices in Intune (Intune で Windows 10 以降のデバイスに Wi-Fi 設定を追加する)</span><span class="sxs-lookup"><span data-stu-id="a6aac-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="a6aac-109">Import Wi-Fi settings for Windows devices in Intune (Intune で Windows デバイス用 Wi-Fi 設定をインポートする)</span><span class="sxs-lookup"><span data-stu-id="a6aac-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="a6aac-110">**一般的な問題**</span><span class="sxs-lookup"><span data-stu-id="a6aac-110">**Common Issues**</span></span>

<span data-ttu-id="a6aac-111">**Wi-Fi プロファイルで指定されている展開済み証明書に依存する Wi-Fi プロファイルを展開しようとしていますが、構成プロファイルにエラー状態が表示されます。**</span><span class="sxs-lookup"><span data-stu-id="a6aac-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="a6aac-112">デバイスが証明書を受信したことを確認します。</span><span class="sxs-lookup"><span data-stu-id="a6aac-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="a6aac-113">Intune で、[**すべてのデバイス**] に移動し、[デバイス]、[**デバイスの構成**] の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="a6aac-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="a6aac-114">すべての必要なプロファイルが表示されていて、状態が正常であることを確認します。</span><span class="sxs-lookup"><span data-stu-id="a6aac-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="a6aac-115">Android プロファイルの場合、証明書チェーンに中間証明書がある場合は、それらの中間証明書が Android デバイスに展開されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="a6aac-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="a6aac-116">証明書の状態を確認するには、[**デバイスの構成**] > [**プロファイル**] > [**Android 中間証明書**] > [**プロパティ**] > [**信頼できる証明書**] の順に移動します。</span><span class="sxs-lookup"><span data-stu-id="a6aac-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="a6aac-117">エラーが引き続き表示される場合は、[手順とトラブルシューティング] セクションを参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6aac-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="a6aac-118">詳細については、「[Overview for troubleshooting SCEP certificate profiles with Microsoft Intune (Microsoft Intune を使用した SCEP 証明書プロファイルのトラブルシューティングの概要)](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6aac-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="a6aac-119">**Wi-Fi プロファイルをデバイスに展開しました。正常に展開されたと Intune に表示されていますが、デバイスが Wi-Fi に接続されていません。**</span><span class="sxs-lookup"><span data-stu-id="a6aac-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="a6aac-120">正常な状態とは、Intune が構成通りにプロファイルを展開したという意味です。</span><span class="sxs-lookup"><span data-stu-id="a6aac-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="a6aac-121">ただし、これらの構成がお使いのネットワークや認証要件に適合していない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="a6aac-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="a6aac-122">接続の試行の詳細については、(Wi-Fi アクセス ポイント コントローラーおよび NPS/Radius サーバー上の) インフラストラクチャと認証サービスのログを確認します。</span><span class="sxs-lookup"><span data-stu-id="a6aac-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="a6aac-123">ログを収集して確認するには、ネットワーク インフラストラクチャ チームまたはサードパーティ Wi-Fi ベンダーと連携する必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="a6aac-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>