---
title: Intune Win32 アプリの展開
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
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/06/2020
ms.locfileid: "48462089"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="f8bfb-102">Intune Win32 アプリの展開</span><span class="sxs-lookup"><span data-stu-id="f8bfb-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="f8bfb-103">Microsoft Intune では、MSI や .EXE を含むもののこれらに限定されない Win32 アプリケーションを Windows 10 デバイスに展開することができます。</span><span class="sxs-lookup"><span data-stu-id="f8bfb-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="f8bfb-104">使用されている展開メカニズムでは、対象デバイスに Intune 管理拡張機能 (IME) が存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f8bfb-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="f8bfb-105">IME は、PowerShell スクリプトまたは win32 アプリケーションの展開をユーザー/デバイスに対象設定すると、自動的にインストールされます。</span><span class="sxs-lookup"><span data-stu-id="f8bfb-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="f8bfb-106">また、以下を含む Win32 アプリを展開するために満たす必要がある前提条件のセットも用意されています。</span><span class="sxs-lookup"><span data-stu-id="f8bfb-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="f8bfb-107">サポートされているプラットフォーム: Windows 10 バージョン 1607 以降 (エンタープライズ、プロ、教育バージョン)。</span><span class="sxs-lookup"><span data-stu-id="f8bfb-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="f8bfb-108">サポートされているアーキテクチャ: x86 と x64。</span><span class="sxs-lookup"><span data-stu-id="f8bfb-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="f8bfb-109">デバイスの管理: AAD 参加と自動登録 (ハイブリッド ドメイン参加やグループ ポリシーの自動登録を含む)。</span><span class="sxs-lookup"><span data-stu-id="f8bfb-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="f8bfb-110">アプリケーション パッケージの形式: [Microsoft Win32 コンテンツ準備ツール](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare)によって準備された .**intunewin** ファイル。</span><span class="sxs-lookup"><span data-stu-id="f8bfb-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="f8bfb-111">制限事項:</span><span class="sxs-lookup"><span data-stu-id="f8bfb-111">Limitations:</span></span>
    - <span data-ttu-id="f8bfb-112">最大サイズ: 8GB。</span><span class="sxs-lookup"><span data-stu-id="f8bfb-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="f8bfb-113">サポートされていないアーキテクチャ: ARM。</span><span class="sxs-lookup"><span data-stu-id="f8bfb-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="f8bfb-114">これらの手順に関連する情報については、ドキュメント「[Add, assign, and monitor a Win32 app in Microsoft Intune (Microsoft Intune での Win32 アプリの追加、割り当て、監視)](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f8bfb-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="f8bfb-115">Win32 アプリを含む Windows でのアプリケーションの展開のトラブルシューティングに関する詳細情報については、以下のドキュメントを参照してください</span><span class="sxs-lookup"><span data-stu-id="f8bfb-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="f8bfb-116">アプリのインストールに関する問題のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="f8bfb-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="f8bfb-117">Win32 アプリのトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="f8bfb-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)