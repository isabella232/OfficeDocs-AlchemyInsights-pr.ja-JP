---
title: Mac または Linux への Microsoft Defender のインストールに関する問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 831060bf45bce5ba6ecb95e244dbfe64641d1b2a
ms.sourcegitcommit: 6cffc12f6f7e6e2efee19e05685f8ee10a823dde
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/17/2020
ms.locfileid: "45160517"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="bc4ee-102">Mac または Linux への Microsoft Defender のインストールに関する問題</span><span class="sxs-lookup"><span data-stu-id="bc4ee-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="bc4ee-103">\*\* Mac \*\*</span><span class="sxs-lookup"><span data-stu-id="bc4ee-103">**Mac**</span></span>

- <span data-ttu-id="bc4ee-104">Microsoft Defender ATP for Mac をインストールする前に、システム要件が満たされていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="bc4ee-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="bc4ee-105">詳細については、[「Microsoft Defender ATP for Macのインストール方法」](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="bc4ee-105">For more info, see [How to install Microsoft Defender ATP for Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="bc4ee-106">ファイル内の情報を確認します。「/Library/Logs/Microsoft/mdatp/install.log」。</span><span class="sxs-lookup"><span data-stu-id="bc4ee-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="bc4ee-107">\*\* Linux \*\*</span><span class="sxs-lookup"><span data-stu-id="bc4ee-107">**Linux**</span></span>

- <span data-ttu-id="bc4ee-108">Linux 用の Microsoft Defender ATP をインストールする前に、システム要件が満たされていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="bc4ee-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="bc4ee-109">詳しくは、[「Microsoft Defender ATP for Linuxのインストール方法」](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="bc4ee-109">For more info, see [How to install Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="bc4ee-110">MDATPサービスが実行されていることを確認するには、[「インストールに失敗しました」](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="bc4ee-110">To verify that MDATP service is running, see [Installation failed](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="bc4ee-111">サービスが実行されていない場合の問題のトラブルシューティングと解決については、[「mdatpサービスが実行されていない場合のトラブルシューティングの手順」](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="bc4ee-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="bc4ee-112">製品の正常性を検証するクライアント構成を確認し、EICAR テキストファイルで検出テストを実行する手順については、[「クライアント構成」](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="bc4ee-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="bc4ee-113">**注**オンアクセスアクティビティでサポートされているファイルシステムのリストについては、[ 「Microsoft Defender ATP for Linux」 ](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="bc4ee-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>