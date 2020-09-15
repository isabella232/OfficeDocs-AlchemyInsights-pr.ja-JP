---
title: Windows 10 の更新プログラムを延期する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1128"
- "6700007"
ms.openlocfilehash: 233354386eb319860f25b3929b6be528438cc865
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680428"
---
# <a name="defer-windows-10-updates"></a><span data-ttu-id="7030a-102">Windows 10 の更新プログラムを延期する</span><span class="sxs-lookup"><span data-stu-id="7030a-102">Defer Windows 10 updates</span></span>

<span data-ttu-id="7030a-103">ユーザーにプッシュされる Windows 10 の更新プログラムを延期するには、次の手順を実行します:</span><span class="sxs-lookup"><span data-stu-id="7030a-103">To defer the Windows 10 updates pushed to users, follow these steps:</span></span>

1. <span data-ttu-id="7030a-104">Azure portal にサインインします。</span><span class="sxs-lookup"><span data-stu-id="7030a-104">Sign in to the Azure portal.</span></span>
2. <span data-ttu-id="7030a-105">**[ソフトウェアの更新]**  >  **[Windows 10 更新リング]** の順に選択します。</span><span class="sxs-lookup"><span data-stu-id="7030a-105">Select  **Software Updates**  >  **Windows 10 Update Rings**.</span></span>
3. <span data-ttu-id="7030a-106">更新リングを持っていない場合は、新規作成オプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="7030a-106">If you don't have an update ring, select the option to create a new one.</span></span>
4. <span data-ttu-id="7030a-107">名前とオプションの説明を入力し、**[設定構成]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="7030a-107">Enter a name and optional description, and then select  **Settings Configure**.</span></span>
5. <span data-ttu-id="7030a-108">異なる更新プログラムを延期するためのタイムフレームをカスタマイズします。</span><span class="sxs-lookup"><span data-stu-id="7030a-108">Customize the timeframe for deferring different updates.</span></span> <span data-ttu-id="7030a-109">最大の延期時間は、更新プログラムの種類によって異なります:</span><span class="sxs-lookup"><span data-stu-id="7030a-109">Maximum deferred time is based on the type of update:</span></span>
    - <span data-ttu-id="7030a-110">**品質更新** はリリースから最大 30 日間延期できます。</span><span class="sxs-lookup"><span data-stu-id="7030a-110">**Quality updates**  can be deferred up to 30 days from their release.</span></span>
    - <span data-ttu-id="7030a-111">**機能更新** はリリースから最大 180 日間延期できます。</span><span class="sxs-lookup"><span data-stu-id="7030a-111">**Feature updates**  can be deferred up to 180 days from their release.</span></span>
