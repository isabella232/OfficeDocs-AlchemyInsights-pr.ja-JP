---
title: Microsoft Edge での Microsoft Defender Application Guard のサポート
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/04/2020
ms.locfileid: "49584218"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a><span data-ttu-id="13d78-102">Microsoft Edge での Microsoft Defender Application Guard のサポート</span><span class="sxs-lookup"><span data-stu-id="13d78-102">Microsoft Edge's support for Microsoft Defender Application Guard</span></span>

<span data-ttu-id="13d78-103">Windows 10 および Microsoft Edge 用に設計された Application Guard は、ハードウェア分離アプローチを使用して、ユーザーがホスト オペレーティング システムから分離された Hyper-V 対応コンテナー内から信頼できないサイトをナビゲートできるようにします。</span><span class="sxs-lookup"><span data-stu-id="13d78-103">Designed for Windows 10 and Microsoft Edge, Application Guard uses a hardware-isolation approach that lets a user navigate an untrusted site from inside an isolated, Hyper-V–enabled container, separated from the host operating system.</span></span>

<span data-ttu-id="13d78-104">エンタープライズ管理者は、信頼済みサイト、クラウド リソース、内部ネットワークの一覧を定義します。</span><span class="sxs-lookup"><span data-stu-id="13d78-104">An enterprise admin defines a list of trusted websites, cloud resources, and internal networks.</span></span> <span data-ttu-id="13d78-105">ユーザーが一覧にないサイトにアクセスすると、そのサイトが Microsoft Edge でコンテナーに表示されます。</span><span class="sxs-lookup"><span data-stu-id="13d78-105">When a user visits a site that's not on the list, Microsoft Edge will open the site in the container.</span></span> <span data-ttu-id="13d78-106">これは、サイトが悪意のあるものであることが判明した場合、ホスト PC は保護され、攻撃者は会社のデータにアクセスできなくなることを意味します。</span><span class="sxs-lookup"><span data-stu-id="13d78-106">This means that if the site turns out to be malicious, the host PC will remain protected and the attacker won't get to the enterprise data.</span></span>

<span data-ttu-id="13d78-107">コンテナーへの拡張機能のインストールは、Microsoft Edge バージョン 81 以降でサポートされており、ポリシーを通して制御できます。</span><span class="sxs-lookup"><span data-stu-id="13d78-107">Installation of extensions in the container is supported as of Microsoft Edge version 81, and it can be controlled via a policy.</span></span> <span data-ttu-id="13d78-108">ポリシーで使用される ExtensionInstallForcelist は、Application Guard が使用するネットワークの分離ポリシーでニュートラル リソースとして追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="13d78-108">The updateURL address that gets used in the ExtensionInstallForcelist policy should be added as a Neutral Resource in the Network Isolation policies used by Application Guard.</span></span>

<span data-ttu-id="13d78-109">詳細については、「[Microsoft Edge での Microsoft Defender Application Guard のサポート](https://go.microsoft.com/fwlink/?linkid=2134229)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="13d78-109">For more info, see [Microsoft Edge support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).</span></span>
