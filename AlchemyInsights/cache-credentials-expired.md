---
title: 'エラー: キャッシュされた資格情報の有効期限が切れているため、変更内容をアップロードまたはダウンロードできません。'
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "3534"
- "9001489"
ms.openlocfilehash: 8105fa7b311bc932f95c8bff4d6b58ed9aabe74a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734484"
---
# <a name="error-we-cant-upload-or-download-your-changes-because-your-cached-credentials-have-expired"></a><span data-ttu-id="a6724-102">エラー: キャッシュされた資格情報の有効期限が切れているため、変更内容をアップロードまたはダウンロードできません。</span><span class="sxs-lookup"><span data-stu-id="a6724-102">Error: We can't upload or download your changes because your cached credentials have expired</span></span>

<span data-ttu-id="a6724-103">OneDrive アプリにファイルを保存するときに、**"キャッシュされている資格情報の有効期限が切れています"** という語句を含むエラーが表示された場合は、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="a6724-103">When saving files to the OneDrive app, if you receive an error that contains the phrase **"your cached credentials have expired"**, perform the following steps:</span></span>

1. <span data-ttu-id="a6724-104">すべての Office アプリケーションを閉じます。</span><span class="sxs-lookup"><span data-stu-id="a6724-104">Close all Office applications.</span></span>
1. <span data-ttu-id="a6724-105">資格情報マネージャーを開き、タスクバーの検索ボックスに「**資格情報マネージャー**」と入力し、[**資格情報マネージャー コントロール パネル**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a6724-105">Open Credential Manager, and type **credential manager** in the search box on the taskbar, then select **Credential Manager Control panel**.</span></span>
1. <span data-ttu-id="a6724-106">[**Windows 資格情報**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a6724-106">Select **Windows Credentials**.</span></span>
1. <span data-ttu-id="a6724-107">"**OneDrive**" という言葉で始まるすべての項目を見つけます。</span><span class="sxs-lookup"><span data-stu-id="a6724-107">Find any entry that starts with the word **OneDrive**.</span></span>
1. <span data-ttu-id="a6724-108">その項目を選択し、[**削除**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a6724-108">Select the entry, then press **Remove**.</span></span>
1. <span data-ttu-id="a6724-109">資格情報マネージャーを閉じ、システムトレイにある青い雲のアイコンを右クリックし、[**OneDrive を終了する**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a6724-109">Close Credential Manager, then right click on the blue cloud in your systray, and select **Close OneDrive**.</span></span>
1. <span data-ttu-id="a6724-110">タスクバーにある検索ボックスに「**OneDrive**」と入力し、[**OneDrive アプリ**] を選択して OneDrive を起動します。 </span><span class="sxs-lookup"><span data-stu-id="a6724-110">Type **OneDrive** into the search box on the taskbar and select **OneDrive App** to launch OneDrive.</span></span>
1. <span data-ttu-id="a6724-111">OneDrive にサインインし、ファイルを OneDrive に保存してみます。</span><span class="sxs-lookup"><span data-stu-id="a6724-111">Sign into OneDrive, then try to save the file to OneDrive.</span></span>
