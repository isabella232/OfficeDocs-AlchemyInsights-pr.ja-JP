---
title: レポートを開くためにレガシ ダイアログの組み込みを有効にする
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: 285933e607ac7e58256709f0c9cf2851250ce211
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806440"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="dc4c2-102">レポートを開くためにレガシ ダイアログの組み込みを有効にする</span><span class="sxs-lookup"><span data-stu-id="dc4c2-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="dc4c2-103">**現象**</span><span class="sxs-lookup"><span data-stu-id="dc4c2-103">**Symptom**</span></span>

<span data-ttu-id="dc4c2-104">ユーザーがレポートを開くことができない。</span><span class="sxs-lookup"><span data-stu-id="dc4c2-104">Users are unable to open reports.</span></span> <span data-ttu-id="dc4c2-105">"問題が発生しました。</span><span class="sxs-lookup"><span data-stu-id="dc4c2-105">"Something has gone wrong.</span></span> <span data-ttu-id="dc4c2-106">詳細については、技術的な詳細を確認してください。"</span><span class="sxs-lookup"><span data-stu-id="dc4c2-106">Check technical details for more details."</span></span>

<span data-ttu-id="dc4c2-107">**原因**</span><span class="sxs-lookup"><span data-stu-id="dc4c2-107">**Cause**</span></span>

<span data-ttu-id="dc4c2-108">"フォーム記述子が null であるか、定義されていません" というエラーが原因で、レポートを UCI に読み込むことができません。</span><span class="sxs-lookup"><span data-stu-id="dc4c2-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="dc4c2-109">UCI のレポートでは現在もレガシ ダイアログが必要であるため、顧客のシステムで *allowlegacydialogsembedding* が有効になっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dc4c2-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="dc4c2-110">**解決方法**</span><span class="sxs-lookup"><span data-stu-id="dc4c2-110">**Solution**</span></span>

1. <span data-ttu-id="dc4c2-111">**[設定] > [管理] > [システム設定] > [全般] タブ**の順に移動します。</span><span class="sxs-lookup"><span data-stu-id="dc4c2-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="dc4c2-112">[統一インターフェイス ブラウザー クライアントに特定のレガシ ダイアログを組み込むことができるようにする] を [**はい**] に設定します。</span><span class="sxs-lookup"><span data-stu-id="dc4c2-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
