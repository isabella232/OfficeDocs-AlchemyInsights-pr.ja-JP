---
title: アプリの互換性テストを行う
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9138"
- "9005291"
ms.openlocfilehash: 9a6a9ea3587a851ecf842588ab73421590ce2431
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2021
ms.locfileid: "50696436"
---
# <a name="do-app-compatibility-testing"></a><span data-ttu-id="4fdbc-102">アプリの互換性テストを行う</span><span class="sxs-lookup"><span data-stu-id="4fdbc-102">Do app compatibility testing</span></span>

<span data-ttu-id="4fdbc-103">Microsoft Edge のアプリケーションの互換性は非常に高いです。</span><span class="sxs-lookup"><span data-stu-id="4fdbc-103">Application compatibility for Microsoft Edge is extremely high.</span></span> <span data-ttu-id="4fdbc-104">実際に、Microsoft が次の互換性の保証を提供するほど、非常に高いレベルです。</span><span class="sxs-lookup"><span data-stu-id="4fdbc-104">In fact, it's so high that Microsoft provides the following compatibility promises:</span></span>
- <span data-ttu-id="4fdbc-105">Microsoft Edge 45 以前のバージョンで動作する場合、Microsoft Edge 77 以降のバージョンでも動作します。</span><span class="sxs-lookup"><span data-stu-id="4fdbc-105">If it works on Microsoft Edge 45 and earlier versions, it will work on Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="4fdbc-106">Internet Explorer で動作する場合は、Internet Explorer モードの Microsoft Edge でも動作します。</span><span class="sxs-lookup"><span data-stu-id="4fdbc-106">If it works on Internet Explorer, it will work on Microsoft Edge in Internet Explorer mode.</span></span>
- <span data-ttu-id="4fdbc-107">Google Chrome で動作する場合、Microsoft Edge で動作します。</span><span class="sxs-lookup"><span data-stu-id="4fdbc-107">If it works on Google Chrome, it will work on Microsoft Edge.</span></span>

<span data-ttu-id="4fdbc-108">この保証を満たしないアプリケーションがある場合、Microsoft アプリ Assure[ 修正することを確約いたします](https://www.microsoft.com/fasttrack/microsoft-365/app-assure)。</span><span class="sxs-lookup"><span data-stu-id="4fdbc-108">If you have an application where we don't meet this promise, then we stand behind the promise to fix it with [Microsoft App Assure](https://www.microsoft.com/fasttrack/microsoft-365/app-assure).</span></span>

<span data-ttu-id="4fdbc-109">こうした確約はあるものの、多くの組織は、コンプライアンスまたはリスク管理の理由で、一部のアプリケーションを検証する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4fdbc-109">Despite this promise, we know that many organizations must validate some applications for compliance or risk-management reasons.</span></span> <span data-ttu-id="4fdbc-110">この手順は非常に簡単になるものと予想していましたが、アプリのテストにおいては組織化され、厳密であることが重要になります。</span><span class="sxs-lookup"><span data-stu-id="4fdbc-110">Even though we expect this to be very straightforward, it's important to be organized and rigorous in app testing.</span></span>

<span data-ttu-id="4fdbc-111">アプリの互換性テストを行うには 2 つの方法があります。</span><span class="sxs-lookup"><span data-stu-id="4fdbc-111">There are two ways to do app compatibility testing:</span></span>

- <span data-ttu-id="4fdbc-112">**ラボ テスト**: アプリケーションは、特定の構成を使用して、厳密にコントロールされた環境でテストされます。</span><span class="sxs-lookup"><span data-stu-id="4fdbc-112">**Lab testing**: Applications are tested in a tightly controlled environment with specific configurations.</span></span>
- <span data-ttu-id="4fdbc-113">**パイロット テスト**: アプリケーションは、限定された数のユーザーが、自分のデバイスを使用し、日常の作業環境の中でテストされます。 </span><span class="sxs-lookup"><span data-stu-id="4fdbc-113">**Pilot testing**: Applications are tested by a limited number of users in their daily work environment using their own devices.</span></span>

<span data-ttu-id="4fdbc-114">各アプリに最も適した方法を選び、組織全体にリリースする前にテストを行います。</span><span class="sxs-lookup"><span data-stu-id="4fdbc-114">Choose the method that is most appropriate for each app and do the testing prior to a launch to the entire organization.</span></span>

<span data-ttu-id="4fdbc-115">アプリと互換性を確認したら、Microsoft Edge をパイロット グループに展開する準備が整ったことになります。</span><span class="sxs-lookup"><span data-stu-id="4fdbc-115">Once you've ensured that your apps are compatible, you're ready to deploy Microsoft Edge to a pilot group.</span></span>
