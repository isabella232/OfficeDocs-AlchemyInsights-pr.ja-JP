---
title: how-to-import-nk2-files
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 83d30b2d62908db791f21ec5ed7fd5537e7a0944
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759337"
---
# <a name="how-to-import-nk2-files"></a><span data-ttu-id="0a243-102">.nk2 ファイルのインポート方法</span><span class="sxs-lookup"><span data-stu-id="0a243-102">How to import .nk2 files</span></span> 

<span data-ttu-id="0a243-103">ユーザーが初めて Microsoft Outlook 2013、Outlook 2016、Outlook 2019 または Outlook for Microsoft 365 を使用するときに、ユーザーのニックネーム キャッシュ (*profilename*.nk2 ファイルに保存されています) が既定のメッセージ ストアの非表示メッセージにインポートされます。</span><span class="sxs-lookup"><span data-stu-id="0a243-103">When you start Microsoft Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365 for the first time, your nickname cache (stored in the *profilename*.nk2 file) is imported into a hidden message in your default message store.</span></span>

<span data-ttu-id="0a243-104">.nk2 ファイルを Outlook 2013、Outlook 2016、Outlook 2019 または Outlook for Microsoft 365 にインポートするために、.nk2 ファイルがフォルダー %appdata%\Microsoft\Outlook にあることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="0a243-104">To import .nk2 files into Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365, make sure that the .nk2 file is in the following folder: %appdata%\Microsoft\Outlook</span></span>

<span data-ttu-id="0a243-105">**注**: .nk2 ファイルの名前は、現在の Outlook 2013 または Outlook 2016 プロファイルと同じ名前にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="0a243-105">**Note**: The .nk2 file must have the same name as your current Outlook 2013 or Outlook 2016 profile.</span></span> <span data-ttu-id="0a243-106">既定では、このプロファイルの名前は "Outlook" です。</span><span class="sxs-lookup"><span data-stu-id="0a243-106">By default, the profile name is "Outlook."</span></span> <span data-ttu-id="0a243-107">プロファイルの名前を確認するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="0a243-107">To check the profile name, follow these steps:</span></span> 
1. <span data-ttu-id="0a243-108">**[スタート]** ボタンをクリックし、**[コントロール パネル]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="0a243-108">Click **Start**, and then click **Control Panel**.</span></span>
2. <span data-ttu-id="0a243-109">**[メール]** をダブルクリックします。</span><span class="sxs-lookup"><span data-stu-id="0a243-109">Double-click **Mail**.</span></span>
3. <span data-ttu-id="0a243-110">[メール設定] ダイアログ ボックスで、**[プロファイルの表示]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="0a243-110">In the Mail Setup dialog box, select **Show Profiles**.</span></span>
4. <span data-ttu-id="0a243-111">**[開始]** > **[実行]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="0a243-111">Select **Start** > **Run**.</span></span>
5. <span data-ttu-id="0a243-112">**[開く]** ボックスで、「*outlook.exe /importnk2*」と入力して **[OK]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="0a243-112">In the **Open** box, type *outlook.exe /importnk2*, and then select **OK**.</span></span> 

<span data-ttu-id="0a243-113">.nk2 ファイルをインポートすると、そのファイルの内容はメールボックスに保存されている既存のニックネーム キャッシュに結合されます。</span><span class="sxs-lookup"><span data-stu-id="0a243-113">After you import the .nk2 file, the contents of the file are merged into the existing nickname cache stored in your mailbox.</span></span>

<span data-ttu-id="0a243-114">**注**: .nk2 ファイルの名前は、Outlook 2013、Outlook 2016、Outlook 2019 または Outlook for Microsoft 365 の次回起動時に .old というファイル拡張子付きに変更されます。</span><span class="sxs-lookup"><span data-stu-id="0a243-114">**Note**: The .nk2 file is renamed with a .old file name extension the next time you start Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365.</span></span> <span data-ttu-id="0a243-115">.nk2 ファイルを再インポートする場合は、最初にファイル拡張子 .old を削除してください。</span><span class="sxs-lookup"><span data-stu-id="0a243-115">If want to re-import the .nk2 file, remove the .old file name extension first.</span></span>

<span data-ttu-id="0a243-116">詳細については、「[オートコンプリートのリストを別のコンピューターにインポートまたはコピーする](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0a243-116">For more information, see [Import or copy the Auto-Complete List to another computer](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).</span></span>