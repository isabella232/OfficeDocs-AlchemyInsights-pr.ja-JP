---
title: Microsoft Edge を Microsoft Intune に追加する
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194654"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="d726b-102">Microsoft Edge を Microsoft Intune に追加する</span><span class="sxs-lookup"><span data-stu-id="d726b-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="d726b-103">Microsoft Edge for Windows 10 を展開、構成、監視、および保護できるようにするには、まず Microsoft Edge を Microsoft Intune に追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d726b-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="d726b-104">Intune は、Microsoft Edge 77 以降のバージョンをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="d726b-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="d726b-105">Intuneは、Microsoft Edge の既存のインストールを検出します。</span><span class="sxs-lookup"><span data-stu-id="d726b-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="d726b-106">Microsoft Edge がユーザー コンテキストでインストールされている場合、システム インストールはユーザー コンテキストでのインストールを上書きします。</span><span class="sxs-lookup"><span data-stu-id="d726b-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="d726b-107">Microsoft Edge がシステム コンテキストでインストールされている場合、インストールの成功が報告されます。</span><span class="sxs-lookup"><span data-stu-id="d726b-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="d726b-108">ユーザー コンテキストのすべてのチャネルに対して、プレインストールされたMicrosoft Edge 77 以降のバージョンは、システム コンテキストにインストールされた Microsoft Edge で上書きされます。</span><span class="sxs-lookup"><span data-stu-id="d726b-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="d726b-109">**前提条件**</span><span class="sxs-lookup"><span data-stu-id="d726b-109">**Prerequisite**</span></span>

<span data-ttu-id="d726b-110">Windows 10 バージョン 1709 以降を実行するコンピューター</span><span class="sxs-lookup"><span data-stu-id="d726b-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="d726b-111">**Intune に Edge を追加する手順**</span><span class="sxs-lookup"><span data-stu-id="d726b-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="d726b-112">[Intune でアプリを構成します](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)。</span><span class="sxs-lookup"><span data-stu-id="d726b-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="d726b-113">[アプリ情報を構成します](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)。</span><span class="sxs-lookup"><span data-stu-id="d726b-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="d726b-114">[アプリの設定を構成します](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)。</span><span class="sxs-lookup"><span data-stu-id="d726b-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="d726b-115">[スコープタグを選択します (オプション)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)。</span><span class="sxs-lookup"><span data-stu-id="d726b-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="d726b-116">[アプリを追加します](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)。</span><span class="sxs-lookup"><span data-stu-id="d726b-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="d726b-117">詳細については、「[トラブルシューティング](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d726b-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




