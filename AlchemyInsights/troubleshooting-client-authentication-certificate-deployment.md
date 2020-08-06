---
title: クライアント認証証明書の展開のトラブルシューティング
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
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/29/2020
ms.locfileid: "46556227"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="37ae6-102">クライアント認証証明書の展開のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="37ae6-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="37ae6-103">Intune の NDES/SCEP クライアント証明書プロファイルおよび PKCS/PFX クライアント証明書プロファイルは、一般的に Wi-Fi、VPN、メールなどのその他のプロファイル タイプと組み合わせて使用され、ユーザーが企業リソースに対して認証できるようにします。</span><span class="sxs-lookup"><span data-stu-id="37ae6-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="37ae6-104">これらのプロファイル タイプがクライアント証明書プロファイルにリンクされるタイミングは、そのプロファイルの正常な展開に依存します。</span><span class="sxs-lookup"><span data-stu-id="37ae6-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="37ae6-105">多くの場合、当初のインフラストラクチャのセットアップとそれに関連するクライアント証明書プロファイルの構成では、トラブルシューティングが必要です。</span><span class="sxs-lookup"><span data-stu-id="37ae6-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="37ae6-106">NDES コネクタを適切にセットアップするための詳しい手順および証明書の展開における問題を特定するためのトラブルシューティングのガイダンスについては、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="37ae6-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="37ae6-107">Configure infrastructure to support SCEP with Intune (Intune を使用してインフラストラクチャを構成して SCEP をサポートする)</span><span class="sxs-lookup"><span data-stu-id="37ae6-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="37ae6-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune (Microsoft Intune を使用した SCEP 証明書プロファイルのトラブルシューティングの概要)</span><span class="sxs-lookup"><span data-stu-id="37ae6-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="37ae6-109">参照されている PowerShell スクリプトを使用して、構成を確認します。</span><span class="sxs-lookup"><span data-stu-id="37ae6-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="37ae6-110">詳細については、「[Intune Certificate connector verification scripts (Intune 証明書コネクタ検証スクリプト)](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="37ae6-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="37ae6-111">**その他の一般的な問題**</span><span class="sxs-lookup"><span data-stu-id="37ae6-111">**Other common issues**</span></span>

<span data-ttu-id="37ae6-112">**Intune 証明書コネクタを NDES コネクタ サーバーにインストールしようとすると、"The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request. (証明書の要求のパスワードを確認できません。そのパスワードが既に使用されている可能性があります。この要求で送信するための新しいパスワードを取得してください。)" というメッセージが表示される。**</span><span class="sxs-lookup"><span data-stu-id="37ae6-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="37ae6-113">このメッセージは、証明書コネクタのインストールを管理者として実行する必要があることを意味します。</span><span class="sxs-lookup"><span data-stu-id="37ae6-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="37ae6-114">一部の環境では、Intune 証明書が実行されるサーバーはプロキシ サーバーを使用して Intune に接続する必要があるため、証明書コネクタ はプロキシを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="37ae6-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="37ae6-115">状況によっては、構成されたプロキシ設定が NDES コネクタによって無視される場合があり、また、LocalSystem のセキュリティ コンテキストでの実行中にプロキシ設定を構成する必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="37ae6-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="37ae6-116">この問題を解決するには、Internet Explorer を SYSTEM として実行し、IE でプロキシを構成します。</span><span class="sxs-lookup"><span data-stu-id="37ae6-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="37ae6-117">Intune コネクタ サービスの再起動後に、NDES コネクタが Intune に接続します。</span><span class="sxs-lookup"><span data-stu-id="37ae6-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="37ae6-118">**ユーザー デバイスが SCEP 証明書を NDES から受信しなくなった。**</span><span class="sxs-lookup"><span data-stu-id="37ae6-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="37ae6-119">NDES サーバーに発行され、NDES コネクタのインストール中に指定されたクライアント認証証明書の有効期限が切れているか欠落している可能性があります。</span><span class="sxs-lookup"><span data-stu-id="37ae6-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="37ae6-120">解決方法:</span><span class="sxs-lookup"><span data-stu-id="37ae6-120">To resolve:</span></span> 
 
1. <span data-ttu-id="37ae6-121">NDES コネクタをアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="37ae6-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="37ae6-122">次の詳細情報を使用して、新しいクライアント認証証明書またはサーバー認証証明書を要求します。</span><span class="sxs-lookup"><span data-stu-id="37ae6-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="37ae6-123">サブジェクト名: CN=external fqdn</span><span class="sxs-lookup"><span data-stu-id="37ae6-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="37ae6-124">サブジェクトの別名 (両方必要です): DNS=external fqdn、DNS=internal fqdn</span><span class="sxs-lookup"><span data-stu-id="37ae6-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="37ae6-125">新しい証明書を使用して NDES コネクタを再インストールします。</span><span class="sxs-lookup"><span data-stu-id="37ae6-125">Reinstall the NDES connector with the new certificate.</span></span>