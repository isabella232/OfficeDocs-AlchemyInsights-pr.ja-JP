---
title: インポート前に .pst ファイルを修復する
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1226"
- "1800027"
ms.assetid: ''
ms.openlocfilehash: 518543f664873c99d5f296284199cd417c620e00
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720142"
---
# <a name="repair-pst-file-before-importing"></a><span data-ttu-id="b7937-102">インポート前に .pst ファイルを修復する</span><span class="sxs-lookup"><span data-stu-id="b7937-102">Repair .pst file before importing</span></span>

<span data-ttu-id="b7937-103">.pst ファイルを Outlook にインポートする前に、以下の手順に従いファイルを修復して、ファイルが破損していないことを確認してください。</span><span class="sxs-lookup"><span data-stu-id="b7937-103">Before you import a .pst file in Outlook, verify the file is not corrupted by repairing the file:</span></span>

1. <span data-ttu-id="b7937-104">Outlook を終了します。</span><span class="sxs-lookup"><span data-stu-id="b7937-104">Exit Outlook.</span></span>

2. <span data-ttu-id="b7937-105">`Scanpst.exe`Office プログラム フォルダー (C:\Program Files (x86)\Microsoft Office\root\Office \<バージョン\>または C:\Program Files\Microsoft Office\root\Office \<バージョン\>) を検索して実行します。</span><span class="sxs-lookup"><span data-stu-id="b7937-105">Find and run `Scanpst.exe` in your Office program folder (C:\Program Files (x86)\Microsoft Office\root\Office\<Version\> or C:\Program Files\Microsoft Office\root\Office\<Version\>).</span></span>

3. <span data-ttu-id="b7937-106">**Microsoft Outlook 受信トレイ修復ツール**で、**[参照]** をクリックして .pst ファイルを検索します (たとえば、C:\Users\\<username\>\AppData\Local\Microsoft\Outlook)。</span><span class="sxs-lookup"><span data-stu-id="b7937-106">In the **Microsoft Outlook Inbox Repair tool**, click **Browse** to find the .pst file (for example, in C:\Users\\<username\>\AppData\Local\Microsoft\Outlook).</span></span> <span data-ttu-id="b7937-107">.pst ファイルを選択し、**[開く]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="b7937-107">Select the .pst file and then click **Open**.</span></span>

4. <span data-ttu-id="b7937-108">**[開始]** をクリックしてスキャンを開始します。</span><span class="sxs-lookup"><span data-stu-id="b7937-108">Click **Start** to begin the scan.</span></span>

5. <span data-ttu-id="b7937-109">ファイルにエラーが見つかった場合は、**[修復]** をクリックし、修復が完了したら **[OK]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="b7937-109">If errors are found in the file, click **Repair**, and then click **OK** when the repair is complete.</span></span>

6. <span data-ttu-id="b7937-110">.pst ファイルを Outlook にもう一度インポートしてみてください。</span><span class="sxs-lookup"><span data-stu-id="b7937-110">Try to import the .pst file in Outlook again.</span></span>

<span data-ttu-id="b7937-111">詳細については、[「Outlook データ ファイルを修復する」](https://support.office.com/article/25663bc3-11ec-4412-86c4-60458afc5253)および[「Outlook .pst ファイルのインポートに関する問題を解決する」](https://support.office.com/article/2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b7937-111">For more information, see [Repair Outlook data files](https://support.office.com/article/25663bc3-11ec-4412-86c4-60458afc5253) and [Fix problems importing an Outlook .pst file](https://support.office.com/article/2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>
