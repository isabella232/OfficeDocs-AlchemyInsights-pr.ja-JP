---
title: OneDrive のクラッシュのトラブルシューティング
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826204"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="8825b-102">OneDrive のクラッシュのトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="8825b-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="8825b-103">OneDrive が繰り返しクラッシュする場合は、次のトラブルシューティングの手順を試してください。</span><span class="sxs-lookup"><span data-stu-id="8825b-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="8825b-104">**レジストリ キーが設定されていないことを確認する:**</span><span class="sxs-lookup"><span data-stu-id="8825b-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="8825b-105">レジストリ エディターを使用して、HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive に移動する</span><span class="sxs-lookup"><span data-stu-id="8825b-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="8825b-106">DisableFileSyncNGSC が存在し、1 に設定されている場合は、キーを開き、値を 0 に変更します。</span><span class="sxs-lookup"><span data-stu-id="8825b-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="8825b-107">スタートに移動して手動で OneDrive を起動する</span><span class="sxs-lookup"><span data-stu-id="8825b-107">Manually launch OneDrive by going to Start</span></span> ![Windows キーを押し、](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="8825b-109">検索ボックスに「OneDrive」と入力して、「OneDrive」デスクトップ アプリをクリックします。</span><span class="sxs-lookup"><span data-stu-id="8825b-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="8825b-110">**OneDrive をリセットする:**</span><span class="sxs-lookup"><span data-stu-id="8825b-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="8825b-111">注:</span><span class="sxs-lookup"><span data-stu-id="8825b-111">Notes:</span></span>

- <span data-ttu-id="8825b-112">OneDrive をリセットすると、(設定されている場合は個人の OneDrive を含む) 既存のすべての同期接続が解除されます。</span><span class="sxs-lookup"><span data-stu-id="8825b-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="8825b-113">お使いのコンピューターで OneDrive をリセットしても、ファイルやデータが失われることはありません。</span><span class="sxs-lookup"><span data-stu-id="8825b-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="8825b-114">**OneDrive をリセットするには:**</span><span class="sxs-lookup"><span data-stu-id="8825b-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="8825b-115">Windows キーと R キーを押し、[実行] ダイアログを開きます。</span><span class="sxs-lookup"><span data-stu-id="8825b-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="8825b-116">「%localappdata%\Microsoft\OneDrive\onedrive.exe /reset 」と入力し、[OK] を押します。</span><span class="sxs-lookup"><span data-stu-id="8825b-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="8825b-117">すぐにコマンド ウィンドウが表示されます。</span><span class="sxs-lookup"><span data-stu-id="8825b-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="8825b-118">スタートに移動して手動で OneDrive を起動する</span><span class="sxs-lookup"><span data-stu-id="8825b-118">Manually launch OneDrive by going to Start</span></span> ![Windows キーを押し、](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="8825b-120">検索ボックスに「OneDrive」と入力して、「OneDrive」デスクトップ アプリをクリックします。</span><span class="sxs-lookup"><span data-stu-id="8825b-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="8825b-121">注:</span><span class="sxs-lookup"><span data-stu-id="8825b-121">Notes:</span></span>

- <span data-ttu-id="8825b-122">リセット前にいくつかのフォルダーのみを同期するように選択した場合、同期の完了後、それを再実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8825b-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="8825b-123">詳細については、「 [コンピューターと同期する OneDrive フォルダーを選択する](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) 」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8825b-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="8825b-124">個人用の OneDrive と OneDrive for Business の場合は、これを完了する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8825b-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>